# drive-and-deliver
Here's where I figure out how an old solution applies to an old industry: TSP/shortest path, and newspaper/mail delivery.

## motivation
Having worked as a paper carrier, and having people close to me depend on paper-carrying as their primary source of income, I believe there is an unquantified amount of pain, discomfort, and wasted effort that accompanies paper delivery, particularly as newspapers downsize and subcontract their physical delivery out to overtaxed local centers. At the same time, the relentless daily nature of paper delivery plus the challenges posed by terrain and urban planning requires   

## requirements (+solutions)
| requirement | sol'n(s) | notes |
| --- | --- | --- |
| correct addresses to location | Google Maps API | |
| street attribute (e.g. directionality/one-ways, lanes) | Google Maps API? | |
| side-of-street distinction | | |
| ability to add own paths | | ***POTENTIALLY DIFFICULT! |
| ability to add custom delivery locations for existing addresses | | e.g. when people's garages OPEN ONTO DIFFERENT STREETS than their front door -_- |
| | *bonus features* | |
| mass input addresses | CSV plugin | Many apps already do this, e.g. OptiMaps, MyRoutePlanner |
| add deliv. details to locations | | e.g. "deliver to front door" |


## existing products
I'm unfamiliar with any solutions and how they measure up against my requirements. I'll begin looking in the following places:
* Major mail delivery companies; UPS, USPS, FedEx
* Amazon?
* The App Stores:
    * Android: [Voyager](https://play.google.com/store/apps/details?id=com.sensis.voyager&hl=en), an app with similar goal and origins; [RoadWarrior](https://www.roadwarriorllc.com), paid iOS + Android app also used by many subcontractors;
    * iOS: [Route4Me](https://itunes.apple.com/us/app/route4me-route-planner/id349853799?mt=8), an app that is apparently used by UPS and others;
    * Web-Based: [OptiMap](https://gebweb.net/optimap/), a web-app that allows for bulk address adding; [MyRouteOnline](https://www.myrouteonline.com), another fairly developed webapp that's explicitly CSV based
    * Other: Navigon by Garmin, apparently 
