# drive-and-deliver
Here's where I figure out how an old problem applies to an old industry: TSP/shortest path, and newspaper/mail delivery.

## motivation
Having worked as a paper carrier, and having people close to me depend on paper-carrying as their primary source of income, I believe there is an unquantified amount of discomfort and wasted effort that accompanies paper delivery, particularly as newspapers downsize and subcontract physical deliveries out to overtaxed local centers. At the same time, the nature of the work plus the challenges posed by terrain and urban planning has limited the efficacy of technological assistance. Though software cannot help the carrier physically move the package from vehicle to destination, there is still much unexplored territory with path optimization that can be covered by software. 

## requirements (+solutions)
| requirement | sol'n(s) | notes |
| --- | --- | --- |
| correct addresses to location | Google Maps API | |
| street attribute (e.g. directionality/one-ways, lanes) | Google Maps API? | *** |
| side-of-street distinction | | *** |
| ability to add own paths | GMaps Roads API; create road segment from drawing on map? | |
| ability to add custom delivery locations for existing addresses | | e.g. when people's garages OPEN ONTO DIFFERENT STREETS than their front door -_- |
| | *bonus features* | |
| mass input addresses | CSV plugin | Many apps already do this, e.g. OptiMaps, MyRoutePlanner |
| add deliv. details to locations | | e.g. "deliver to front door" |
| traffic annotations | | traffic generally doesn't impact carriers, as deliveries either happen during off-peak hours or have date deadlines, not time deadlines. However, traffic closures could still be relevant. |

#### *** = a note on Google Maps Roads API.
It appears that Google Maps represents roads in a very low-level manner: as geometrically calculated vectors. 

e.g.: one way roads
"If the nearest road is one-way, one segment is returned." https://developers.google.com/maps/documentation/roads/nearest

## existing products
I'm unfamiliar with any solutions and how they measure up against my requirements. I'll begin looking in the following places:
* Major mail delivery companies; UPS, USPS, FedEx
* What does Amazon use for internal package delivery? Would it be applicable to door-to-door delivery at all?
* Waze's capabilities
* The App Stores:
    * Android: [Voyager](https://play.google.com/store/apps/details?id=com.sensis.voyager&hl=en), an app with similar goal and origins; [RoadWarrior](https://www.roadwarriorllc.com), paid iOS + Android app also used by many subcontractors;
    * iOS: [Route4Me](https://itunes.apple.com/us/app/route4me-route-planner/id349853799?mt=8), an app that is apparently used by UPS and others;
    * Web-Based: [OptiMap](https://gebweb.net/optimap/), a web-app that allows for bulk address adding; [MyRouteOnline](https://www.myrouteonline.com), another fairly developed webapp that's explicitly CSV based
    * Other: Navigon by Garmin, apparently 
