---
layout: post
title:      "Coindesk Scraper - Coding Takeaways "
date:       2019-04-09 16:50:30 +0000
permalink:  coindesk_scraper_-_coding_takeaways
---


In this project, I built a ruby gem that scrapes the top news from Coindesk. It collects a list of news articles from the Coindesk homepage and gives users a CLI that they can interact with, eg. pulling the full article based on the user’s choice or review the list of articles. The knowledge applied here includes Ruby language, Object Oriented programming and Scraping.

There are a few takeaways from developing the gem that I’d like to share. I used the Outside In development approach in developing the gem. It is a CLI program, so I started by thinking how I want my users to interact with my program. As a first step, I tried to figure out the interface I would like my users to have, such as having a greeting, brief information about the gem and an instruction on what they can do next.

The part that I believe that laid the basis for my program is the code structure. Objects interact with each other through the developer’s own design. I began by laying out my file structures and my target outcomes. For example, I would like to have a CLI file that gives instructions to the user and accepts user’s inputs; I would also like to have a controller file which runs my codes to return the targeted outputs; lastly I would need a scraping file the whole job of which is to scrape from the website. In addition, because I would want to assign properties to my news articles, such as a title, a release date and a URL, and call them when needed, it comes handy if I program my news article objects as instance and assign the properties as my instance’s attributes. 

Along the way as I coded, I applied some basic coding principles. When having my classes communicating with each other, I tried to use less objects. It is much easier to maintain and keep the most flexibility of codes if one object serves only one job. Also, functions like loop are the key to keep a program interactive – You would want your users to keep being engaged and playing with your program instead of making it a one-time thing.  There are also small things that I took notes on, such as watch out for the return value of a method, sequence of the codes matters, test run frequently, commit early and commit often, use dummy codes to test the operational structure first... 

The last thing I'd like to mention is scraping. When scraping, it is really important to take a moment and analyze the structure of the webpage first and see how the webpage breaks down into sections and expands its content. For example, on the Coindesk website, the content of its home page is clustered into three sections: top-article, featured-articles, and article-streams. After understanding the structure, it becomes ituitive to know how to use CSS Selector to select the specific elements to iterate over in my program.

Last but not least, coding sometimes can be overwhelming and exhausting. From the way I see, code structure is always more important than the code itself. The key is to understand clearly the goal and the designed outcome and then start from there. Just like in life, take one step at a time in coding, and you know you will get there.

Happy coding!
