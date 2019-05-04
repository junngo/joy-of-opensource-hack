# Episode 6
Apr 26 - May 4, 2019  
Commenting Issue, Code Analysis, Submitting patches

## Links
* [Bug 1517993](https://bugzilla.mozilla.org/show_bug.cgi?id=1517993)-An unexpected error occurred with browser.cookies.set() with domain and url key for ip addresse
* [Submitting patches](https://phabricator.services.mozilla.com/D29933)

## Topics
* If you write domain key in set function, It is domain cookies(It is not host-only).
* IP addresses are not domain names. I should check cookies domain wheather is IP addresses.
* If host(i.e. cookie.host) is IP address(IPv6 or IPv4), the host(i.e. cookie.host) be not added a leading ".". 

## Keywords
* Cookie
* JS test - mochitest
