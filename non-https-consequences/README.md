## Motiviation

This document discusses the consequences of serving a web page non-securely in the next years. (Security concerns completely put aside)

## Browsers will mark non-secure origins as non-secure
[https://www.chromium.org/Home/chromium-security/marking-http-as-non-secure](https://www.chromium.org/Home/chromium-security/marking-http-as-non-secure)

### Non-secure
![image](https://cloud.githubusercontent.com/assets/474248/9668783/dbfe99e2-5283-11e5-8f26-b9227a6dcd94.png)

### Secure
![image](https://cloud.githubusercontent.com/assets/474248/9668823/10f01cd4-5284-11e5-9cd7-f5848212c310.png)

## New web apis are going to be https only

 - [Service Workers](http://www.w3.org/TR/service-workers/#security-considerations)
  - background tasks
  - geofencing
  - push notifications
  - new cache abilities
 - [App install banners](https://developers.google.com/web/updates/2015/03/increasing-engagement-with-app-install-banners-in-chrome-for-android?hl=en) (due to service worker being needed)
 
http://www.w3.org/TR/service-workers/#security-considerations

## Existing web apis will stop working non secure
 - geolocation
 - access to microphone / camera
 - full screen
 - (session) storage
 
https://sites.google.com/a/chromium.org/dev/Home/chromium-security/deprecating-powerful-features-on-insecure-origins

https://sites.google.com/a/chromium.org/dev/Home/chromium-security/prefer-secure-origins-for-powerful-new-features

http://www.w3.org/TR/powerful-features/#feature-requires-privilege

https://blog.mozilla.org/security/2015/04/30/deprecating-non-secure-http/

### Deprecation already in process
Using geolocation on non-secure origin already utters a deprecation warning in recent Chrome versions.
![image](https://cloud.githubusercontent.com/assets/474248/9669024/1f0dbd48-5285-11e5-86cd-0403b156aabb.png)
