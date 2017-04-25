# External API Developer Notes

Here at GA we have compiled notes from our developer students about the APIs they have used.  Hopefully these notes will help guide you in your work with external APIs.

## General

This is where general API notes/advice will go.

## Spotify

And this is where specific API notes will go.

Try to include links and pictures wherever possible.


## Sound Cloud
This API was not the easiest to work with. Their descriptions on how to use the callbacks were there but not with proper examples.
Here is a small example of what I am talking about:
![https://developers.soundcloud.com/docs/api/guide#search]

They were really helpful in using the Widget to play music and what was needed to set up and or play the playlists/tracks you wanted.
![https://developers.soundcloud.com/docs/api/html5-widget]

The JSON data is very detailed and you can do a lot with the data that comes back if you are needing to do things in particular, ie: genres, BPM, users, comments...

My suggestion is to actually not use SoundCloud as a 3rd party API, why you may be asking? Well this is a old Dinosaur so if you think about it the data is not updated often or if at all, there is lacluster support for use with JS, however Ruby and Python are well documented. If you are looking for a music API to use check out Spotify...they at least have a tool to see the exact callbacks you can do and how to get the data you will need.

There are a lot of things you will need to make this API work with the Widget. You need to connect to the SDK on your HTML. You should copy and paste their SC initialization for the widget here: ![https://w.soundcloud.com/player/api.js], plus if trying to figure out the extra info you need you will have to figure out the OAuth and token information which there is NO JS support.

Please keep in mind that they will take longer than 1 month for API approval. So if you are wanting to use this API you should consider it for maybe project 3 when you are looking for API's for project 2. 