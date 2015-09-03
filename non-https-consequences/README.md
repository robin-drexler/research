## Motiviation

This document discusses the consequences of serving a web page by http instead of https.(Security concerns completely put aside)

## Browsers will mark non-secure origins as non-secure
[https://www.chromium.org/Home/chromium-security/marking-http-as-non-secure](https://www.chromium.org/Home/chromium-security/marking-http-as-non-secure)

### Non-secure
![image](https://cloud.githubusercontent.com/assets/474248/9668783/dbfe99e2-5283-11e5-8f26-b9227a6dcd94.png)

### Secure
![image](https://cloud.githubusercontent.com/assets/474248/9668823/10f01cd4-5284-11e5-9cd7-f5848212c310.png)

## New web apis are going to be https only

 * [Service Workers](http://www.w3.org/TR/service-workers/#security-considerations)
 * [App install banners](https://developers.google.com/web/updates/2015/03/increasing-engagement-with-app-install-banners-in-chrome-for-android?hl=en) (due to service worker being needed)

[Mozilla outlines](https://blog.mozilla.org/security/2015/04/30/deprecating-non-secure-http/), that they're plan to add new features https only.

## Existing web apis will stop working non secure
...
