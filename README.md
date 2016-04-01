# jQuery.cookiebar
Based on PrimeBox jQuery CookieBar Plugin - [Site](http://www.primebox.co.uk/projects/jquery-cookiebar/)

##Installing

To start, download the zip file containing the Cookie Bar plugin, a CSS file and example HTML document. Upload the javascript and CSS files to your website and add them between your head tags. Make sure to download the latest version of jQuery if your website does not already include it.

First add in your HTML the references to the js file and to the default CSS.

```html
<script type="text/javascript" src="/your-js-folder/jquery.js"></script> 
<script type="text/javascript" src="/your-js-folder/jquery.cookiebar.js"></script> 
<script type="text/javascript"> 
  $(document).ready(function(){
     $.cookieBar();
  });
</script>
```

You will also need to initialise the Cookie Bar, which can be done with the following code (Make sure if you already use $(document).ready() that you only copy what you need of below so you don't have too many $(document).ready()'s).

```javascript
$(document).ready(function(){
  $.cookieBar();
});
```

##Disabling Google Analytics and other cookies
If a user chooses to disable cookies (If you give them that option), you need to make sure that scripts such as Google Analytics need to be disabled.
This can be done by wrapping the code in a simple if statement.

```javascript
if(jQuery.cookieBar('cookies')){
  //Google Analytics or other code here
}
```

##Options
There are a number of options allowing you to customise how the plugin works:

```javascript
message: 'We use cookies to track usage and preferences',
acceptButton: true,
acceptText: 'I Understand',
acceptFunction: null,
declineButton: false,
declineText: 'Disable Cookies',
declineFunction: null,
policyButton: true,
policyText: 'Privacy Policy',
policyURL: '/privacy-policy/',
autoEnable: true,
acceptOnContinue: false,
acceptOnScroll: false,
acceptAnyClick: false,
expireDays: 365,
renewOnVisit: false,
forceShow: false,
effect: 'slide',
element: 'body',
append: false,
fixed: false,
bottom: false,
zindex: '',
domain: 'www.example.com',
referrer: 'www.example.com',
'ignore': 'ignore-this-class'
```

##License

Copyright © 2016 Martino Lessio - [Website](http://www.martinolessio.com)

This library is based on the plugin originally made by PrimeBox. Attribution follows. Thanks to those guys.

This work is licensed under the Creative Commons Attribution 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by/3.0/.

When using this software you use it at your own risk. We hold no responsibility for any damage caused by using this plugin or the documentation provided.

### Attribution
Copyright (C) 2012 PrimeBox (info@primebox.co.uk)
  
This work is licensed under the Creative Commons Attribution 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by/3.0/.
  
Documentation available at:
http://www.primebox.co.uk/projects/cookie-bar/
  
When using this software you use it at your own risk. We hold no responsibility for any damage caused by using this plugin or the documentation provided.
