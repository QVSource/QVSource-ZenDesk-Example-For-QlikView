ZenDesk Example App For QlikView
================================
An example application showing how to get started using the [QVSource General Web Connector](http://wiki.qvsource.com/General-Web-Connector-For-QlikView.ashx) for QlikView & Qlik Sense configured for the ZenDesk API.

*Note that the [load script](https://github.com/QVSource/QVSource-ZenDesk-Example-For-QlikView/blob/master/QVSource-ZenDesk-Example-For-QlikView-prj/LoadScript.txt) should also work in Qlik Sense.*

This demo currently pages through all the tickets in ZenDesk and loads some of the basic data for each and then stores the results into a QVD file.

Suggested improvements include:
* Making requests to other parts of the ZenDesk API to look up the values behind links such as the requester_id, assigneed_id, organization_id etc.
* More intelligent updates, for example to only get tickets from the past week (and accumulate them into the QVD file).

If you are a QlikView + QVSource user you can simply click the ["Download ZIP"] (https://github.com/QVSource/QVSource-ZenDesk-Example-For-QlikView/archive/master.zip) button on GitHub to grab this application.

The content below is copied from the change log in the first tab of the load script.

![](screenshot1.png)

Change Log
----------
1.0.4 - 01/11/15
----------------
* Switched to using the Zendesk Incremental API (https://developer.zendesk.com/rest_api/docs/core/incremental_export#tickets) which is recommended 'To get a list of all tickets in your account' (see here - https://developer.zendesk.com/rest_api/docs/core/tickets#listing-tickets).
* Also switched to using the JsonToXmlRaw table which makes it easier to get all the data in a single request.
* Removed reference to an external credentials.txt file.
* Added a MonthYear dimension.
* Added variables to set load access token (for QVSource Web Edition) and app ID.

1.0.3 - 07/09/15
----------------
* Added empty QVDs folder.

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
