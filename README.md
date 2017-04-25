# External API Developer Notes

Here at GA we have compiled notes from our developer students about the APIs they have used.  Hopefully these notes will help guide you in your work with external APIs.

## General

Request an authentication key as early as possible.  Some companies can take weeks to approve you.

Check potential APIs for documentation on query parameters and route info.  If they don't have much at all, it might be wise to look for something else.

See if the API you're interested in has been updated regularly/recently; if it hasn't, you might find a lot of bugs and missing data.  Also, the information might be outdated.



## Spotify

The Spotify API has excellent documentation and the ability to test out the majority of endpoints in the site:
#[](https://developer.spotify.com/web-api/search-item/)

However!  If you want to use multiple parameters in one request or get more in depth song info (such as tempo, duration) you will have to use token authorization and that is a very complicated process.  There is a tutorial for setting up a Spotify login through a server but after that the process gets very complex.
Example:
#[](https://developer.spotify.com/web-api/get-audio-analysis/)
Authorization Documentation:
#[](https://developer.spotify.com/web-api/authorization-guide/)

To embed a player into your page use this: 
#[](https://developer.spotify.com/technologies/widgets/spotify-play-button/)


