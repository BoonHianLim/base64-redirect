# Base-64 Redirect

This is a proof of concept to show that it is possible to do a "url shortener" with static pages using query parameter.

To test this, base64 encode any url in the format of either:
* www.google.com 
* google.com 
* https://www.google.com

Then, append it to the end of the github page url, for example:

https://boonhianlim.github.io/base64-redirect?redirect=d3d3Lmdvb2dsZS5jb20= 

The above link will redirect you to Google.

Have Fun!

## Concept

The idea of this codebase is since url shortener is such a popular design problem, I would like to check if it is possible to  implement the base-64 approach for shortening the URL in a static website.

Technically we should have use a mapping between the unique ID in the database to match with the website, then use base62 / base64 encoding to convert the id. However, in static website, there isn't a easy way to just store something without starting a server. The easiest approach is just to base64 encoded the link itself. Technically this is not a shortner but more of a redirect, hence the name.