# Client Storage Strategies

- Local Storage
- Session Storage
- IndexedDB
- Web SQL
- Cookies
- Application Cache

## Local Storage  
The read-only localStorage property allows you to access a Storage object for the Document's origin; the stored data is saved across browser sessions. localStorage is similar to sessionStorage, except that while data stored in localStorage has no expiration time, data stored in sessionStorage gets cleared when the page session ends — that is, when the page is closed.
- Data stored in sessionStorage is specific to the protocol of the page. In other words, http://example.com will have separate storage than https://example.com.
- Keys and values are always strings.
- No sensitive information should be stored.
- LocalStorage limit across all browsers is 5 MB.
- localStorage.setItem('key', 'value')
- localStorage.getItem('key')
- localStorage.removeItem('key')
- localStorage.clear()
- localStorage.length

## Session Storage
The sessionStorage property accesses a session Storage object for the current origin. sessionStorage is similar to localStorage; the difference is that while data in localStorage doesn't expire, data in sessionStorage is cleared when the page session ends.
- A page session lasts as long as the browser is open, and survives over page reloads and restores.
- Opening a page in a new tab or window creates a new session with the value of the top-level browsing context, which differs from how session cookies work.
- Opening multiple tabs/windows with the same URL creates sessionStorage for each tab/window.
- Closing a tab/window ends the session and clears objects in sessionStorage.
- Data stored in sessionStorage is specific to the protocol of the page.
- sessionStorage.setItem('key','value')
- sessionStorage.getItem('key')
- sessionStorage.removeItem('key')
- sessionStorage.clear()
- sessionStorage.length

## IndexedDB
IndexedDB is a low-level API for client-side storage of significant amounts of structured data, including files/blobs. It uses indexes to enable high-performance searches of this data. While Web Storage is useful for storing smaller amounts of data, it is less useful for storing larger amounts of structured data. IndexedDB provides a solution.
 IndexedDB API is powerful, but may seem too complicated for simple cases. If you'd prefer a simple API, try libraries such as localForage, dexie.js, ZangoDB, PouchDB, idb, idb-keyval and JsStore that make IndexedDB more programmer-friendly.
 IndexedDB is a transactional database system, like an SQL-based RDBMS, but instead of fixed-column tables it uses js based object oriented database.
 Any object supported by the [structured clone algorithm ](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Structured_clone_algorithm) can be stored.  
Well it's a [long](https://developers.google.com/web/ilt/pwa/working-with-indexeddb) [long](https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API/Using_IndexedDB) journey.

## Web SQL  
Web SQL specification defining an API for storing data in databases that can be queried using a variant of SQL. The W3C stopped actively maintaining the Web SQL spec in 2010 and has no plans to maintain it any further.
Consider replacing your Web SQL database with a modern alternative, such as IndexedDB.
- [The link](https://www.w3.org/TR/webdatabase/)

## Cookies  

## Application Cache


### Footnote
1. Welcome ajinkya
2. Dashboard ( Time, Work Timeline, weather, Language )
3. To do Form ( To do and time )
4. live news ( every 5 min refresh )
5. Reminders ( food, imp works, calls, mails )
6. Calendar Events
