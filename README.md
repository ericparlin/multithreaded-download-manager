[![Mozilla Add-on](https://img.shields.io/amo/v/multithreaded-download-manager.svg?style=flat-square)](https://addons.mozilla.org/firefox/addon/multithreaded-download-manager/) [![Mozilla Add-on](https://img.shields.io/amo/d/multithreaded-download-manager.svg?style=flat-square)](https://addons.mozilla.org/firefox/addon/multithreaded-download-manager/)

## Multi-threaded download manager
#### Firefox 57 Extension: Support for multi-threaded download manager
##### *Experimental - use at your own risk*
###### The downloaded file will be saved to Firefox's internal storage and then moved to the default download directory. Make sure there is enough storage space.
###### It is recommended that all download tasks are deleted or paused before exiting the browser, restarting, updating, etc... 
###### If the browser's out-of-process-extension flag is disabled, an error will occur after a file download completes. The extension can automatically correct this error, but requires an extra file copy. This can also cause the download notification/popup to be blank-resizing of notification will fix this.
###### Firefox has a limit on the number of simultaneous connections to the same server. If more than 6 threads are required go to **__about:config__** and increase the value of 'network.http.max-persistent-connections-per-server' and 'network.http.max-persistent-connections-per-proxy'.
###### This extension requires Firefox's internal storage (indexedDB), so it does not work in "Always use private browsing" mode.
###### This extension can download files using multiple connections. This may increase download speed depending on network conditions.
###### Click the toolbar button to open the download panel, or right-click the button to open it in a new tab or window. Click the button at the bottom of the panel or create a new download task in the context menu of the download link.
###### The monitor download function can be enabled in the extension options page. When enabled, opening a file larger than the specified size will automatically pop up the download dialog. Selecting "Continue in Browser" switches to the browser's built-in downloader.
