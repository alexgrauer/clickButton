ClickButton
===========
 
A library that decodes multiple clicks on one button. Also copes with 
long clicks and click-and-hold. 
 
Usage:
-------

```
ClickButton buttonObject(pin [LOW/HIGH, [CLICKBTN_PULLUP]],TRUE/FALSE);
```
 
where LOW/HIGH denotes active LOW or HIGH button (default is LOW) 
CLICKBTN_PULLUP is only possible with active low buttons. 
TRUE/FALSE denotes if the button will report when released or not. (default is FALSE)
 
Returned click counts:
----------------------

   A positive number denotes the number of (short) clicks after a released button
   A negative number denotes the number of "long" clicks
   A positive number(100 + number of clicks) denotes when the button was released if the option was set to TRUE

