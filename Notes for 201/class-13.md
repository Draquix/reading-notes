## Notes Day 12 -- From html link
[Source File](http://diveinto.html5doctor.com/storage.html)

Native client applications have space for storage easily allocated.  Cookies 
were one of the first implementations of local storage for web applications but
they store very small bits of data.  They are included in every HTTP request and
that slows things down, and it isn't encrypted, and are limited to 4kb.

IE had a larger userdata storage allocation. No one uses IE anymore.  Flash
allowed 'flash cookies' which were 100kb objects, one per domain. We don't use
Flash anymore. A browser plugin Gears gave space for SQL tables... every method
relies on a platform specific or third party plugin.

HTML5 Storage allows for storing data of key/value pairs locally within the web
browser that persists after navigating away from the page. The first step of 
utilizing it is to check if the browser supports it, as below function.

    function supports_html5_storage() {
        try {
            return 'localStorage' in window && window['localStorage'] !== null;
        } catch (e) {
            return false;
        }
    }

We store key/value pairs. the key is a string, the value is any data type in
javascript, but it's stored as a string, so retrieval needs to use functions 
like parseInt(). It requires: 
    
    var foo = localStorage.getItem("bar");  //and respectively 
    localStorage.setItem("bar",foo);

Tracking changes to local storage requires listening for an event that fires 
when something is changed.
Each origin gets 5mb of storage space.  In the future SQL-like commands may be 
able to be used through javascript.

[Back to Table of Contents](../README.md)