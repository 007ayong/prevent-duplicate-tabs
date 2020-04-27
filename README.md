## About

Simple add-on for prevent duplicate tabs, you can custom this using options in popup

![promocional](promo.png)

## Requirements

- Chrome 30+
- Firefox 48+
- Opera 40+

## Install

- [Opera](https://addons.opera.com/en/extensions/details/prevent-duplicate-tabs/)
- [Firefox](https://addons.mozilla.org/en-US/firefox/addon/smart-prevent-duplicate-tabs/)

## Configs

### Sort order

- **Close olders**

    Closes the oldest repeated tabs

- **Keep the tab that is active**

    Don't close active tabs

### Events

- **start**

    Close repeated tabs when your browser is launched

- **update**

    Close repeated tabs when a tab is updated, more details in [`tabs.onUpdated.addListener`](https://developer.chrome.com/extensions/tabs#event-onUpdated)

- **create**

    Close repeated tabs when a new tab is created, more details in [`tabs.onCreated.addListener`](https://developer.chrome.com/extensions/tabs#event-onCreated)

- **remove**

    Close repeated tabs when a tab is closed, more details in [`tabs.onRemoved.addListener`](https://developer.chrome.com/extensions/tabs#event-onRemoved)

- **replace**

    Close repeated tabs when a tab is replaced with another tab due to prerendering or instant, more details in [`tabs.onReplaced.addListener`](https://developer.chrome.com/extensions/tabs#event-onReplaced)

- **datachange**

    Close repeated tabs when you change **sort order**, **events**, **urls** and **others** configurations from extension

### URLs

- **only http**

    Close only tabs with HTTP(s) urls

- **querystring**

    If disabled (off) it's ignore querystring in URLs, then this `http://foo/bar?baz` will be equivalent to this `http://foo/bar`

- **hash**

    If disabled (off) it's ignore hash in URLs, then this `http://foo/bar#baz` will be equivalent to this `http://foo/bar`

### Others

- **incognito**

    Check repeated anonymous tabs (requires you to manually enable in your browser)
