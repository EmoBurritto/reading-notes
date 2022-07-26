# Local Storage and How To Use It On Websites
 
HTTP as the main transport layer of the Web is bad because it is stateless

everytime you close an application it restores to its default 

server-side, and you would check the user name to know which state to revert to

use cookies: 

They add to the load of every document accessed on the domain.
They allow up to only 4 KB of data storage.
Because cookies have been used to spy on people’s surfing behavior, security-conscious people and companies turn them off or request to be asked every time whether a cookie should be set.

localStorage.setItem('favoriteflavor','vanilla');

local storage can only store strings in the different keys; objects need to be defined

(reference:https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)
## Questions 

1. Why would a developer use local storage for a web application?

in order to keep it severside and not restore defaults when reuploaded, keep a key 

2. What information should not be stored in local storage?

never put personal user info, some cookies save without user knowledge 

3. Local storage can store what type of data? How would you convert it to that type before storing?

strings, JSON.stringify() and JSON.parse()

## Things I want to Know More About
-  why people do cookies that people don't know about 
- when to locally store projects in real life
- will it be done in this class?
