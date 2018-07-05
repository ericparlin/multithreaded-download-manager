[![Mozilla Add-on](https://img.shields.io/amo/v/multithreaded-download-manager.svg?style=flat-square)](https://addons.mozilla.org/firefox/addon/multithreaded-download-manager/) [![Mozilla Add-on](https://img.shields.io/amo/d/multithreaded-download-manager.svg?style=flat-square)](https://addons.mozilla.org/firefox/addon/multithreaded-download-manager/)

# Multithreaded Download Manager

Experimental Firefox 57 extension: download manager with multithreading support.

#### Important note:

* **This extension is experimental. Use at your own risk.**
* The requested file is first downloaded to Firefox's internal storage and then moved to the default download folder. Make sure there is enough disk space.
* It is suggested to remove or pause all the tasks before exiting Firefox or performing updates. The extension can resume downloads after the update or the next start of Firefox (losing only about 1 second's progress), though this feature is less tested.
* If the feature "out of process extensions" (enabled by default in Windows, disabled by default in Linux) is disabled, the browser will have problem saving the downloaded file. The extension can workaround it but an additional copy is required. It may also cause the popup window to be blank (resizing can fix it).
* Firefox limits the number of simultaneous connections to a single server. If more than 6 threads are needed, increase network.http.max-persistent-connections-per-server and network.http.max-persistent-connections-per-proxy in about:config .
* The extension requires access to the internal storage (indexedDB) and does not work with the "always private browsing" mode without granting exceptions


This extension can download files with multiple connections to the server. Depending on the network condition, this may increase the download speed.

Click the toolbar button to open the download panel. Alternatively, right click the button to open in a new tab or window. Download tasks can be created by clicking the buttons at the bottom of the panel, or in the context menu of links on websites.
Monitoring download can be enabled in the options. When it is enabled, files larger than a configured size will automatically trigger the download dialog. Click "continue in browser" to switch to Firefox's built-in download.

---
