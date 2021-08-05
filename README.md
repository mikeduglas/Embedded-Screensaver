# Embedded-Screensaver
Embedded screensaver is like system screensaver - it is launching if a user is inactive for some period (no mouse or keyboard input).  
Unlike system screensaver, embedded one is running inside your program, keeping your opened windows away from prying eyes while you have lunch.  
  
The package includes 4 sample screensavers: Floating Text, Digital Clock, Static Image, and Ball Fusion, but you can easily add your owns.  

## Template
Just add global extension and local extension to WINDOW procedure, usually it is Main Appframe procedure.
![Screensaver template](https://github.com/mikeduglas/Embedded-Screensaver/blob/master/template1.png?raw=true)  
![Screensaver template](https://github.com/mikeduglas/Embedded-Screensaver/blob/master/template2.png?raw=true)  

## Features
- Password protected screensaver.

## Demo app
The demo is standard School application. Run the program and leave your computer alone for 10-12 seconds to see the effect, 
or select Test item from Screensaver menu to run active screensaver immediately.  
  
All 4 screensavers are available.

### Floating Text
Customizable options: text, font, size, style, text color, speed.
![Floating text](https://github.com/mikeduglas/Embedded-Screensaver/blob/master/floatingtext.png?raw=true)  

### Digital Clock
Customizable options: font, size, style, color, time format.
![Digital clock](https://github.com/mikeduglas/Embedded-Screensaver/blob/master/clock.png?raw=true)  

### Ball Fusion
Customizable options: text, font, size, style, text color, speed.
![Ball Fusion](https://github.com/mikeduglas/Embedded-Screensaver/blob/master/ballfusion.png?raw=true)  

### Static Image
Customizable options: image file.

## Conceptual example

```
  PROGRAM
  INCLUDE('scrsvr.inc'), ONCE
  MAP
  END
Window                        WINDOW('Caption'),AT(,,361,210),GRAY,FONT('Segoe UI',9),RESIZE
                                ENTRY(@s20),AT(34,56),USE(?ENTRY1)
                                BUTTON('Button1'),AT(140,55),USE(?BUTTON1)
                                BUTTON('Close'),AT(304,182,46),USE(?bClose),STD(STD:Close)
                              END
im                            TIdleMonitor
ss                            TScreenSaverFloatingText
  CODE
  OPEN(Window)
  im.Init(Window, 5, ss)
  ACCEPT
  END
```

## Requirements
- Windows 2000 and higher
- C6 and higher, ABC/Legacy
- No dependencies

## Price
- $100 [PayPal](https://www.paypal.me/mikeduglas?ppid=PPC000628&cnac=RU&rsta=ru_RU(ru_RU)&cust=8W29QJ6GKY9HS&unptid=75f96da6-24a4-11e9-ae2c-441ea14e9560&t=&cal=ff0291196b3f5&calc=ff0291196b3f5&calf=ff0291196b3f5&unp_tpcid=ppme-social-user-profile-created&page=main:email&pgrp=main:email&e=op&mchn=em&s=ci&mail=sys)