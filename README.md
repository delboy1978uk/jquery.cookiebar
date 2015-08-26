# jquery.cookiebar
Stick it to the EU Government with this compliant cookie bar

It's a paradox. "If you dont want tracking cookies, click here to let us know you dont want tracked, and we'll place a tracking cookie on your computer that tracks you noting the fact that you dont want tracked.". What a lot of nonsense. 

This jquery plugin is a githubbed fork of http://www.primebox.co.uk/projects/cookie-bar/ 

Usage
-----
```javascript
<script type="text/javascript">
	$(document).ready(function(){
		$.cookieBar({
			bottom: true;
		});
	});
</script>
```
Options
-------
```javascript
message: 'We use cookies to track usage and preferences.', //Message displayed on bar
acceptButton: true, //Set to true to show accept/enable button
acceptText: 'I Understand', //Text on accept/enable button
declineButton: false, //Set to true to show decline/disable button
declineText: 'Disable Cookies', //Text on decline/disable button
policyButton: false, //Set to true to show Privacy Policy button
policyText: 'Privacy Policy', //Text on Privacy Policy button
policyURL: '/privacy-policy/', //URL of Privacy Policy
autoEnable: true, //Set to true for cookies to be accepted automatically. Banner still shows
acceptOnContinue: false, //Set to true to silently accept cookies when visitor moves to another page
expireDays: 365, //Number of days for cookieBar cookie to be stored for
forceShow: false, //Force cookieBar to show regardless of user cookie preference
effect: 'slide', //Options: slide, fade, hide
element: 'body', //Element to append/prepend cookieBar to. Remember "." for class or "#" for id.
append: false, //Set to true for cookieBar HTML to be placed at base of website. YMMV
fixed: false, //Set to true to add the class "fixed" to the cookie bar. Default CSS should fix the position
bottom: false, //Force CSS when fixed, so bar appears at bottom of website
zindex: '', //Can be set in CSS, although some may prefer to set here
redirect: String(window.location.href), //Current location
domain: String(window.location.hostname), //Location of privacy policy
referrer: String(document.referrer) //Where visitor has come from
acceptFunction: false, //Callback function that triggers when user accepts
declineFunction: false, //Callback function that triggers when user declines
```
