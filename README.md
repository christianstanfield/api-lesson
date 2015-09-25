# Connecting to an API

We're going to learn how to integrate an API into our existing site. For the purpose of this lesson let's assume your app is a food and travel blog, and you want to include information from Yelp on your site relevant to your articles.

## 1) Research APIs
Check out the list of APIs on this website: http://www.programmableweb.com. It’s pretty inclusive and has links to their respective sites.

Once you've explored it a bit, take a look at the page for Yelp: http://www.programmableweb.com/api/yelp.

## 2) Read the documentation
Read over the documentation for the Yelp API: https://www.yelp.com/developers/documentation/v2/search_api. We’re going to be making GET requests to their server for information to add to our blog.

## 3) Try their API console
Yelp has a handy interactive console on their website to try out making requests: https://www.yelp.com/developers/api_console. Try making a few different queries and look closely at the data that you get back.

## 4) Understand the gem
Follow the link to the ruby gem for the Yelp API: https://www.yelp.com/developers/documentation/v2/examples. This will make it easier for us to make requests by creating ruby objects and methods that we can use in our application. Take a look at the provided documentation in the readme file.

## 5) Investigate the gem source code
Besides reading the documentation, also take a look at the source code to more fully understand how the gem is working and what it’s doing for you: https://github.com/Yelp/yelp-ruby/blob/develop/lib/yelp/endpoint/search.rb.

## 6) Setup a Yelp app
Follow the instructions on Yelp’s website to register an app under your account.

## 7) Include gem and initializer
Add the gem and initializer to your rails project per the instructions in the documentation.

## 8) Add fields to the database
We’re going to want to save search terms for each of our articles so that we can make requests to Yelp and display the results on our website alongside our writing. Add at least two new fields to your articles table, one for location and another for food. Also add the corresponding fields to the new article form and controller params.

## 9) Write a blog post
It doesn’t have to be anything fancy but write a brief blog post about something food or travel related so that we have an example to use. Make Anthony Bourdain proud :)

## 10) Create controller method
Before we display our new page we want to make a request to Yelp with those new database fields. Write a method to accomplish that and call it from your controller action in article show.

## 11) Update view content
Finally add some placeholders on your view to display the content from Yelp. If you have time, style it to make it look nice.
