A ShareKit plugin for Hyves by Peperzaken.

**INTRODUCTION**

This service uses the Hyves Data-API. To get started on working with the Data-API, you need to follow a couple of simple steps. For more information see the getting started section in Hyves' Data-API documentation: http://www.hyves-developers.nl/documentation/data-api/getting-started. Note: this service currently only uses the tips.create method in the Hyves Data-API to share items (http://www.hyves-developers.nl/documentation/data-api/methods/1.2/tips.create).

**GETTING STARTED**

1. Place the ShareKit folder in your project.
2. Add the following frameworks if they are not already included:

	* MessageUI
	* Security
	* SystemConfiguration

3. Register your application at Hyves (steps are described at http://www.hyves-developers.nl/documentation/data-api/getting-started)
4. Add your Hyves consumer- and secret-key to SHKConfig.h like below:

```
	#define SHKHyvesConsumerKey			@"CONSUMER_KEY_HERE"
	#define SHKHyvesSecretKey			@"SECRET_KEY_HERE"
```

5. You are done. To actually share an item:

```
	// Create a shareable ShareKit item
	SHKItem* item = [SHKItem text:@"Hyves service example test in ShareKit by Peperzaken http://peperzaken.nl/over-peperzaken."];

	// Share the item through the SHKHyves service
	[SHKHyves shareItem:item];
```

6. For additional documentation, check ShareKit's full documentation: http://getsharekit.com/docs/.
7. Have fun. :-)

```
MMMMMMMMMMMMMMMMMMMMMOOOZ$$$$$$$$$ZOOOOMMMMMMMMMMMMMMMMMMMMM
MMMMMMMMMMMMMMMDOOZ$$$$$$$$$$$$$$$$$$$$$ZOODMMMMMMMMMMMMMMMM
MMMMMMMMMMMMMNDOZ$$$$$$$$$$$$$$$$$$$$$$$$$ZOONMMMMMMMMMMMMMM
MMMMMMMMMMMDOZ$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$ZONMMMMMMMMMMM
MMMMMMMMMD8O$$$$$$$$$$$$$$$$$$$$$+?7$$$$$$$$$$$$ODMMMMMMMMMM
MMMMMMMNOZ$$$$$$$$$$$$$$$$$$$$$?,.~I$$$$$$$$$$$$$ZONMMMMMMMM
MMMMMM8Z$$$$$$$$$$$$$$$$$$$$$$7+.=7$$$$$$$$$$$$$$$$Z88MMMMMM
MMMMMMZ$$$$$$$$$$$$$$$$$$$$$$$$?,=I$$$$$$$$$$$$$$$$$ZOMMMMMM
MMMN8O$$$$$$$$$$$$$$$$$$$$$$?:.....,?$$$$$$$$$$$$$$$$$8DMMMM
MMMDZ$$$$$$$$$$$$$$$$$$$$$$?:. ......=$$$$$$$$$$$$$$$$ZDMMMM
MMMZ$$$$$$$$$$$$$$$$$$$$$$$,   ........$$$$$$$$$$$$$$$$ZOMMM
MMDZ$$$$$$$$$$$$$$$$$$$$$$$.   ........7$$$$$$$$$$$$$$$ZONMM
MNO$$$$$$$$$$$$$$$$$$$$$$$$    ........I$$$$$$$$$$$$$$$$$DNM
DZ$$$$$$$$$$$$$$$$$$$$$$$$$    ........I$$$$$$$$$$$$$$$$$ZDM
8Z$$$$$$$$$$$$$$$$$$$$$$$$$    ........I$$$$$$$$$$$$$$$$$ZDM
I$$$$$$$$$$$$$$$$$$$$$$$$$$.   ........7$$$$$$$$$$$$$$$$$$7=
7$$$$$$$$$$$$$$$$$$$$$$$$$$,   ........7$$$$$$$$$$$$$$$$$$7+
7$$$$$$$$$$$$$$$$$$$$$$$$$$,   ........$$$$$$$$$$$$$$$$$$$7I
7$$$$$$$$$$$$$$$$$$$$$$$$$$:   ........$$$$$$$$$$$$$$$$$$$7I
7$$$$$$$$$$$$$$$$$$$$$$$$$$~   ......,~$$$$$$$$$$$$$$$$$$$7I
7$$$$$$$$$$$$$$$$$$$$$$$$$$=...      :I$$$$$$$$$$$$$$$$$$$7+
8Z$$$$$$$$$$$$$$$$$$$$$$$$$=...     .~$$$$$$$$$$$$$$$$$$$$7=
8Z$$$$$$$$$$$$$$$$$$$$$$$$$~...     +$$$$$$$$$$$$$$$$$$$$Z8M
DZ$$$$$$$$$$$$$$$$$$$$$$$$$:...     I$$$$$$$$$$$$$$$$$$$$ZDM
MNO$$$$$$$$$$$$$$$$$$$$$$$$....   ,~$$$$$$$$$$$$$$$$$$$$$DMM
MMDZ$$$$$$$$$$$$$$$$$$$$$I:....  ~?$$$$$$$$$$$$$$$$$$$$ZONMM
MMMZ$$$$$$$$$$$$$$$$$$$$I=.......I$$$$$$$$$$$$$$$$$$$$$ZOMMM
MMM8Z$$$$$$$$$$$$$$$$$$$......,=$$$$$$$$$$$$$$$$$$$$$$ZDMMMM
MMMMDO$$$$$$$$$$$$$$$7+,......?$$$$$$$$$$$$$$$$$$$$$$$8NMMMM
MMMMMMZ$$$$$$$$$$$7+:.....,I$$$$$$$$$$$$$$$$$$$$$$$$ZOMMMMMM
MMMMMMDZ$$$$$$$$$$,...,:+7$$$$$$$$$$$$$$$$$$$$$$$$$Z8NMMMMMM
MMMMMMMNDZ$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$ZONMMMMMMMM
MMMMMMMMMN8O$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$8NMMMMMMMMMM
MMMMMMMMMMMMOZ$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$ZOOMMMMMMMMMMMM
MMMMMMMMMMMMMMNOZ$$$$$$$$$$$$$$$$$$$$$$$$$ZOONMMMMMMMMMMMMMM
MMMMMMMMMMMMMMMN8OZ$$$$$$$$$$$$$$$$$$$$$ZO8DMMMMMMMMMMMMMMMM
MMMMMMMMMMMMMMMMMMMMM8OOOZ$$$$$$$$ZOO88MMMMMMMMMMMMMMMMMMMMM
MMMMMMMMMMMMMMMMMMMMMMMMMO=======~?MMMMMMMMMMMMMMMMMMMMMMMMM
```