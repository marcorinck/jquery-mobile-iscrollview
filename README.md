This is a fork of the original [https://github.com/watusi/jquery-mobile-iscrollview](jquery-mobile-iscrollview) 
project by [https://github.com/watusi](watusi). 

The only difference to the original project is, that the javascript file now is an amd module which can be loaded 
by requireJS.

###Installation

* Download [lib/jquery.mobile.iscrollview.js](lib/jquery.mobile.iscrollview.js) OR
* Install via bower: `bower install jquery-mobile-iscrollview-amd`

Its best to define a shim for this lib like so: 

````javascript
require.config({
		paths:{
		  ....
		},
		shim:{
			'iscroll':{ deps:['jquery'], exports:'iscroll' },
			'iscrollview':{ deps:['jquery.mobile', 'iscroll'], exports:'iscrollview' },
		}
});
````


###Changelog

**1.3.3**
* first version of fork based on original version 1.3.3
* changed the lib to be amd compatible
* registered this fork as a bower package
