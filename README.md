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

The idea of this codebase is since url shortener is such a popular design problem, I would like to check if it is possible to  implement the base-64 approach for shortening the URL in a static website. Seems working.