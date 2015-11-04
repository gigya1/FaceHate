# FaceHate
Google Chrome extension for modifying HTTP headers in web requests to Facebook  

FaceHate was created as a proof of concept extension for Google Chrome to modify HTTP headers:
- User Agent (UA)
- Cookie
- Referer 
in the HTTP packets sent to Facebook servers (to increase privacy). 

The problem is that user cannot login to Facebook (it is obvious as the cookies are constantly changed). 
However it would be great to add functionality to the extension, such that when user browse the Internet (non-Facebook page) all headers are changed, if user navigates to Facebook portal - only UA is changed. 

The extension is based on chrome.webRequest API. I tried to combine it with chrome.Tabs API to get the URL from address bar and use it as condition in handler. It did not work as the API is asynchronous. 
I also tried to create content.js which retrieved URL via window.location.host and pass it via chrome.runtime.sendMessage to background.js as condition in handler. It also did not work. 

Any suggestions?


