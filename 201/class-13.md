# Local Storage

![Image](
https://i.ytimg.com/vi/k8yJCeuP6I8/maxresdefault.jpg)

### Definition and Usage
- The localStorage properties allow to save key/value pairs in a web browser.

- The localStorage object stores data with no expiration date. The data will not be deleted when the browser is closed, and will be available the next day, week, or year.

- The localStorage property is read-only.

### Syntax

**Syntax for SAVING data to localStorage:**

    localStorage.setItem("key", "value");

**Syntax for READING data from localStorage:**

    var lastname = localStorage.getItem("key");

**Syntax for REMOVING data from localStorage:**

    localStorage.removeItem("key");

![Image](
https://res.cloudinary.com/practicaldev/image/fetch/s--rSskJpsi--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/i/2imjutnczd4f3jdhgbdx.png)
    

## THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS

- Persistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.

- Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:

-Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over  
-Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)  
-Cookies are limited to about 4 KB of data — enough to slow down your application , but not enough to be terribly useful

## HTML5 STORAGE

*So what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.*

![Image](
https://clementbuchanan.github.io/reading-notes/images/html5.jpg)

## USING HTML5 STORAGE
**HTML5** Storage is based on named **key/value** pairs.  
 You store data based on a named key, then you can retrieve that data with the same key.  
  The named key is a string. The data can be any type supported by JavaScript, including **strings**, **Booleans**, **integers**, or **floats**. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like **parseInt()** or **parseFloat()** to coerce your retrieved data into the expected JavaScript datatype.

  ### STORAGEEVENT OBJECT

  PROPERTY | TYPE | DESCRIPTION 
----|-----
key |string| the named key that was added, removed, or modified 
oldValue |any| any	the previous value (now overwritten), or null if a new item was added 
newValue |any| any	the new value, or null if an item was removed 
url* |string| the page which called a method that triggered this change


## HTML5 Web SQL Database (Past)
- The Web SQL Database was an initial attempt by vendors to bring SQL-based relational databases to the browser. It has been implemented in Chrome, Safari and Opera 15+, but was opposed by Mozilla and Microsoft in favor of IndexedDB.

- **The advantages of Web SQL Database:**

-designed for robust client-side data storage and access  
-it uses SQL like many server side applications  
-some support on Webkit/Blink desktop and mobile browsers  

- **The disadvantages:**

-SQL never seemed appropriate for client-side development  
-the database schema must be defined up-front  
-marginal browser support and the Webkit/Blink teams may eventually drop it  
-the W3C specification was abandoned in 2010  
-In summary: don’t use a Web SQL Database!  


## HTML5 Web Storage (Present and Future)
- Web Storage provides two objects with identical APIs: **window.localStorage** to retain persistent data
**code.sessionStorage** to retain session-only data which is lost when the tab is closed.
- Domain-specific strings are stored using name/value pairs. Unlike cookies, the storage limit is far larger (at least 5MB) and information is never transferred to the server.

### BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS
- While the past is littered with hacks and workarounds, the present condition of HTML5 Storage is surprisingly rosy.  
- A new API has been standardized and implemented across all major browsers, platforms, and devices.  
- As a web developer, that’s just not something you see every day, is it? But there is more to life than “5 megabytes of named key/value pairs,” and the future of persistent local storage is… how shall I put it