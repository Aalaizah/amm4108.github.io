Title: RSS Feeds in ofCourse and Ghost.org
Date: 2015-4-21 19:47
Category: Development
Tags: HFOSS, BizLeg

#### ofCourse
ofCourse is an open source courseware. It's something that we're using for some of the courses in the Open Source minor. It is a location where students can share cool information that they've found as well as an easy to find location for the professor to post important information. These classes have a blogging requirement within them, so one of the pages on the courseware is the participants page. This page contains links to each of our completed homework assignments as well as a count of how many total blog posts we have. 

##### RSS Feeds
The blog count is done through the RSS feeds of each persons individual blogs. However, with the current version, it does not handle all allowed versions of RSS feeds. As is seen in the [RSS specifications](http://tools.ietf.org/html/rfc5005#section-3) paginating the RSS feed is a legitimate 

#### Ghost.org
Ghost is an open source, and simple to use, blogging system. You can host your blog on their website [Ghost.org](https://ghost.org) or you can host it pretty much anywhere else you might want to. In the most recent release version of Ghost, the RSS feed is generated paginated if you have more than 15 posts. While this normally would be fine, it's not implemented entirely correctly. Each page of the RSS feed should point to the page that came before it, as well as the page that comes after it if they exist. 

#### The Class
All of these have lead to a major problem for me in my open source classes. We're already way past needing to have 15 blog posts in both classes. So the combination of Ghost's incorrect implementation of the RSS feed and ofCourses lack of dealing with a paginated feed anyways means I have pretty much two options. I can spend the time to do a deep dive into two different projects and fix both of them, or I can migrate my class posts to a new blog location. 

#### My Decision
While having both of these projects as things that I could point to and say I worked on these would be awesome, I just don't honestly have the time to work on them. I already have some other personal projects that I think will teach me more for where I want to go on top of having a ton of school work. Because of this I have decided, for the time being at least, that I'm just going to mirror my class posts on a second blog.

#### Pelican
Along with deciding to create a second blog for this class, I had to figure out a second blogging platform to use. While there are a ton of different reasons to pick any blogging platform, I decided on Pelican. This was mostly a decision of convenience as the people who were around me at the time that I made the choice both use it and were able to help me get everything set up.