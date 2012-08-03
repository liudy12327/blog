blog
====
There are two models in this test blog, user and post. 
If the names of the users appear in the select menu in the add post page
the association is connected.
These are the tables for the blog_2.2:

CREATE TABLE `posts` (


`id` int(11) unsigned NOT NULL auto_increment,


`name` varchar(255) default NULL,


`date` datetime default NULL,


`content` text,


`user_id` int(11) default NULL,


PRIMARY KEY (`id`)


);



CREATE TABLE `users` (


`id` int(11) unsigned NOT NULL auto_increment,


`name` varchar(100) default NULL,


`email` varchar(150) default NULL,


`firstname` varchar(60) default NULL,


`lastname` varchar(60) default NULL,


PRIMARY KEY (`id`)


);
