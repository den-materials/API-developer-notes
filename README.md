# External API Developer Notes

Here at GA we have compiled notes from our developer students about the APIs they have used.  Hopefully these notes will help guide you in your work with external APIs.

# General

Request an authentication key as early as possible.  Some companies can take weeks to approve you.

Check potential APIs for documentation on query parameters and route info.  If they don't have much at all, it might be wise to look for something else.

See if the API you're interested in has been updated regularly/recently; if it hasn't, you might find a lot of bugs and missing data.  Also, the information might be outdated.

## TheySaidSo.com/api

A Database of quotes! Authors, Politicians, all around great minds...  If You like quotes this is a great resource.

They self describe as the "Greatest Quotes Api on Earth", but I don't really care about that. Their documentation is excellent and this api is extremely easy to work with.  There are a lot of search parameters you can include too like length and data type.
	I recommend it for anyone who wants an API that won't make their projects harder to complete -- which I appreciate even more now that I got to see how people truly struggled with crappy api's.

Downside is it cost $5 / mo if you make more than 10 pulls a day.

## Sound Cloud
This API was not the easiest to work with. Their descriptions on how to use the callbacks were there but not with proper examples.
Here is a small example of what I am talking about:
https://developers.soundcloud.com/docs/api/guide#search

They were really helpful in using the Widget to play music and what was needed to set up and or play the playlists/tracks you wanted.
https://developers.soundcloud.com/docs/api/html5-widget

The JSON data is very detailed and you can do a lot with the data that comes back if you are needing to do things in particular, ie: genres, BPM, users, comments...

My suggestion is to actually not use SoundCloud as a 3rd party API, why you may be asking? Well this is a old Dinosaur so if you think about it the data is not updated often or if at all, there is lacluster support for use with JS, however Ruby and Python are well documented. If you are looking for a music API to use check out Spotify...they at least have a tool to see the exact callbacks you can do and how to get the data you will need.

There are a lot of things you will need to make this API work with the Widget. You need to connect to the SDK on your HTML. You should copy and paste their SC initialization for the widget here: https://w.soundcloud.com/player/api.js, plus if trying to figure out the extra info you need you will have to figure out the OAuth and token information which there is NO JS support.

Please keep in mind that they will take longer than 1 month for API approval. So if you are wanting to use this API you should consider it for maybe project 3 when you are looking for API's for project 2. 

# Spotify API

The Spotify API has excellent documentation and the ability to test out the majority of endpoints in the site:
#[](https://developer.spotify.com/web-api/search-item/)

However!  If you want to use multiple parameters in one request or get more in depth song info (such as tempo, duration) you will have to use token authorization and that is a very complicated process.  There is a tutorial for setting up a Spotify login through a server but after that the process gets very complex.
Example:
#[](https://developer.spotify.com/web-api/get-audio-analysis/)
Authorization Documentation:
#[](https://developer.spotify.com/web-api/authorization-guide/)

To embed a player into your page use this: 
#[](https://developer.spotify.com/technologies/widgets/spotify-play-button/)

## Co Trails

For this app I used the api "TrailAPI" from the site Mashape. While this api includes alot about trails around the world, it needs the npm library 'unirest' to function. There is documentation on unirest through npmjs.com, however its very exensive and time consuming to learn how to use it in 5 days. I also searched for tutorials on using unirest while buildiung restful routes and found one guy who was using Angular. Try not to use unirest.

### Meetup.com API 

This API provides some great information about meetups and events. However, while some things are documented well there is a pretty solid portion that is not. There is not a list of query options you can add to your query, only the end points you can go too. The end points provide some good information but many of them you must know a lot of details about the event to make the query. Most of the data you will get will be fairly general as it is really hard to narrow searches without knowing the query parameters. If you are willing to tinker and find out what information you are looking for and filter it yourself. Then check out this API, it is not that bad. Tip use api v3, &radius= and &topic_catagory=   are your friends. 

## PetFinder

Easy to use API that returns data in JSON or XML depending on preference. The documentation provides you with ample descriptions of how to receive the type of data you want to and lets you hone in on specifics like age, location, breed, type of animal, etc. The data comes back with all the information you could possibly want to know about each animal along with image links, contact information and detailed descriptions.

The documentation provides you with examples of the routes you'll need to use to get back the information you want.

APIs don't need to be ruff.

https://www.petfinder.com/developers/api-docs

## ShopStyle API

ShopStyle is a great API for anyone that wants to access multiple retailers & clothing items all from one source.  Some examples are Nordstrom, Shopbop, etc.  The API returns JSON and is pretty straightforward but has a LOT of information to sort through so it's a great idea to think through your specific goals before diving in.  Getting the key is pretty easy, all you have to do is create an account through ShopStyle and they generate an API key that you can access through your account settings.  Here is a link to the API overview with directions:

https://www.shopstylecollective.com/api/overview

## Mashape

This API library has a lot of great api's to choose from along with great documentation. The only problem is that Mashape uses the unirest library for the requests, which we haven't covered yet. Besides the unirest issue, Mashape is a great place to find an api. 

Mashape's documentation comes along with examples for each request which is nice. Also Mashape provides the endpoints to test in PostMan which is very helpful. 

https://www.mashape.com/

## GOOGLE MAPS API
-------------------
by alex:
highly recommend this api, great instructions online and lots of room for expansion and personalization. just takes a second to get used to their 'specific' commands, in this sense reading the documentation is essential otherwise you might be banging your head against the wall like "WHY CAN'T I GET THE LATITUDE WHEN I'M SAYIN .LAT", because it's not quite as simple as that. Like I said, highly recommend. 10/10 would use again.
