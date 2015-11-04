# FaceHate
Google Chrome extension for modifying HTTP headers in web requests to Facebook  

FaceHate was created as a proof of concept extension for Google Chrome to modify HTTP headers:
- User Agent
- Cookie
- Referer 
in the HTTP packets sent to Facebook servers. 

The problem is that user cannot login to Facebook (it is obvious as the cookies are changed). 
However it would be great to add functionality to the extension, such that when user browse the Internet (non-Facebook page) the headers are changed, if 
