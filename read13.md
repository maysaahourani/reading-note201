# LOCAL STORAGE FOR WEB APPLICATIONS
 Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:

1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

**What we really want is** no more cookies

1. a lot of storage space
2. on the client
3. that persists beyond a page refresh
4. and isn’t transmitted to the server

Before HTML5, all attempts to achieve this were ultimately unsatisfactory in different ways.



# INTRODUCING HTML5 STORAGE [“Local Storage” or “DOM Storage.”]

So what is HTML5 Storage?

 Simply put, it’s a way for web pages to store named 
 *key/value*  pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

 # HTML5 storage
 HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats.


 Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-existent key will return null rather than throw an exception.

 var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);

There are also methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).

`` interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();``
  Calling removeItem() with a non-existent key will do nothing.

Finally, there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).

``interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};``






