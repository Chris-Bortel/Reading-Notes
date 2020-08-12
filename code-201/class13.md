# Past present and future of local storage applications
<br>
[GitHub Repo](https://github.com/Chris-Bortel/Reading-Notes)

## cookies
- cookies were the early source of storage.
- they are not the best
  - cookies slow down web app by transmitting data over and over.
cookies send unencryted daya over the internet.
cooks are limited to 4kb: enough to be slow and note enough to be useful

## what we want!
- a lot of storage space
on the client
that persists beyond a page refresh
and isn’t transmitted to the server

## solutions before html5
- There were many of them, but all of them were either sigle browser specific, or relied on a third-party plugin.

## The problem that html5 was working on
to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.

## Using HTML5 Storage
- key value pairs
- if you are storing anything other than srings, you need to use functions like parseInt() or parseFloat
local storage is an object. just use square brackets... Check out the snippet

```
var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;
```



