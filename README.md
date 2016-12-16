WinHTTP Proxy Status
====================
This sample demonstrates how to use the WinHTTP API core functionality for querying the proxy settings to determine the proxy for a particular URL.

The APIs demonstrated in this sample are:

1. WinHttpGetProxyForUrl

2. DetectAutoProxyUrl


Both [**WinHttpGetProxyForUrl**](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384097) and [**WinHttpGetProxyForUrlEx**](http://msdn.microsoft.com/en-us/library/windows/desktop/hh405356) are used in this sample. These functions implement the Web Proxy Auto-Discovery (WPAD) protocol for automatically configuring the proxy settings for an HTTP request. The WPAD protocol downloads a Proxy Auto-Configuration (PAC) file, which is a script that identifies the proxy server to use for a given target URL. PAC files are typically deployed by the IT department within a corporate network environment. These functions can automatically discover the location of the PAC file on the local network.

This sample can be extended as needed for your application, using the proxy code from this sample as a starting point, to add additional functionality. For example, an application could add a per-URL proxy cache, awareness for network changes, a filter for bad proxies, or other desired functionality.

Related technologies
--------------------
[Windows HTTP Services (WinHTTP)](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384273)

Related topics
--------------
[WinHttpOpenRequest](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384099)

[WinHttpCreateProxyResolver](http://msdn.microsoft.com/en-us/library/windows/desktop/hh405355)

[WinHttpFreeProxyResult](http://msdn.microsoft.com/en-us/library/windows/desktop/hh707321)

[WinHttpGetProxyResult](http://msdn.microsoft.com/en-us/library/windows/desktop/hh707322)

[WinHttpGetProxyForUrlEx](http://msdn.microsoft.com/en-us/library/windows/desktop/hh405356)

[WINHTTP\_PROXY\_INFO](http://msdn.microsoft.com/en-us/library/windows/desktop/aa383912)




Build the sample
----------------
To build the sample using Visual Studio:

1.  Open Windows Explorer and navigate to the **\\cpp** directory.

2.  Double-click the icon for the **WinhttpProxyStatus.sln** file to open the file in Visual Studio.

3.  In the **Build** menu, select **Build Solution**. The application will be built in the default **\\Debug** or **\\Release** directory.


Run the sample
--------------
To run the sample:

1.  Navigate to the directory that contains the new executable, using the command prompt.

2.  Type **WinhttpProxyStatus.exe \<url\>** at the command prompt.

