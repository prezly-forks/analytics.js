# About Analytics.js

Analytics.js makes it easy to collect customer data and send it to many different tools using a single, unified API.
The end goal of this Analytics.js fork is to only build `PrezlyIntegration` integration so our customers can use the Prezly analytics.js which has the identical api and payload as Segment.com analytics.js

## Building
```js
npm run build
```

It will generate:
- analytics.js - Useful for including into a already established build process
- analytics.min.js - To be hosted on CDN so customers can just embed it

## Usage

Following snippet of code will be enough for customer to start submitting events to Prezly API:

```js
    analytics.init({
        Prezly: {
            apiHost: "//press.prezly.dev/segment",
        },
    });

    analytics.page();
```
