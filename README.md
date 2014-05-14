ZenDesk Example App For QlikView
================================
An example application showing how to get started using the [QVSource General Web Connector](http://wiki.qvsource.com/General-Web-Connector-For-QlikView.ashx) for QlikView configured for the ZenDesk API.

This demo currently pages through all the tickets in ZenDesk and loads some of the basic data for each and then stores the results into a QVD file.

Suggested improvements include:
* Making requests to other parts of the ZenDesk API to look up the values behind links such as the requester_id, assigneed_id, organization_id etc.
* More intelligent updates, for example to only get tickets from the past week (and accumulate them into the QVD file).

If you are a QlikView + QVSource user you can simply click the ["Download ZIP"] (https://github.com/QVSource/QVSource-ZenDesk-Example-For-QlikView/archive/master.zip) button on GitHub to grab this application.

The content below is copied from the change log in the first tab of the load script.

1.0.2 - 14/05/14
----------------
* Added additional comments to credential section.
* Renamed some variables for clarity.
* Now caches API response for an hour (optional line to uncomment which will clear the cache).
* Moved QVSource URL into variable vRoot.

1.0.1 - 04/12/13
----------------
* Added badge.

1.0.0 - 09/10/13
----------------
* Initial Release
