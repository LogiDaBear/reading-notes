# Reading Notes for Class 13
## Local Storage and How To Use It On Websites
[Local Storage and How To Use It On Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)
1. Why would a developer use local storage for a web application?
Because HTTP is stateless and resets when its closed whereas local storage is much simpler with a JS modification to `localStorage` object, You can also use `sessionStorage` instead of `localStorage` if you want the data to be maintained only until the browser window closes.

2. What information should not be stored in local storage?
PII, authentication keys, user locations and API keys 

3. Local storage can store what type of data? How would you convert it to that type before storing? 
It stores key-value pairs in a browser with no expiration date. Before you store it they need to be converted as strings


## Things I want to know more about
Tracking changes in HTML5 storage via strorage event objects. [Main page.](http://diveinto.html5doctor.com/storage.html) Specifically [this paragraph.](http://diveinto.html5doctor.com/storage.html#storage-event).