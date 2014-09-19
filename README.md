There are two types of users:
	
	- Blog Administrator 
		
		modify/delete posts,comments
		enter new posting..
		
	- Blog Users
		visit the blog site
		enter comments about particular postings

First of all, we create new rails project:
	
	$rails new blog

Then, we use scaffold generator ( to create the MVC components needed for posts and comments)

	for posts;

	$rails generate scaffold post title:string body:text

	for comments;

	$rails generate scaffold comment post_id:integer body:text

Finally, we run following commands:

	$rake db:migrate
	$rake routes (Optinal. It shows path routes)
	$rails server
