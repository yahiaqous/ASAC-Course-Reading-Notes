# Local Storage for Web Applications


## BEFORE HTML5

**Cookies** were invented early in the web’s history, and they can be used for persistent local storage of small amounts of data. But they have three potentially deal-breaking downsides:
* Cookies are included with every HTTP request, thereby **slowing down** the web application by needlessly transmitting the same data over and over
* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet
* Cookies are limited to about **4 KB** of data — enough to slow down the application, but not enough to be terribly useful


In the beginning, Microsoft invented a great many things and included them in their browser, **Internet Explorer**, one of these things was called **DHTML Behaviors**, and one of these behaviors was called **userDat**a which allows web pages to store up to **64 KB** of data per domain

In 2007, Google launched **Gears**, an open-source browser plugin aimed at providing additional capabilities in browsers


## HTML5

**HTML5 Storage**: a way for web pages to store named key/value pairs locally, within the client web browser


## Limitations in Current Browsers

the limitations of the now-standardized HTML5 Storage:
* “**5 megabytes**” is how much storage space each origin gets by default
* “**QUOTA_EXCEEDED_ERR**” is the exception that will get thrown if the storage quota exceeds 5 megabytes