# Embedded-Screensaver
Embedded screensaver is like system screensaver - it is launching if a user is inactive for some period (no mouse or keyboard input).  
Unlike system screensaver, embedded one is running inside your program, keeping your opened windows away from prying eyes while you have lunch.  

The demo is standard School application. Run the program and leave your computer alone for 10-12 seconds to see the effect.  
2 screensavers are available inside School app - basic (default) and Ball Fusion. You can choose one or another from the menu.  

[Download the demo](https://yadi.sk/d/nox5p_Hhq3SgCg)  
**If you are not able to download from the link above, drop me private message and I will send you a zip.**  

## Conceptual example

>   PROGRAM
>   INCLUDE('scrsvr.inc'), ONCE
>   MAP
>   END
> Window                        WINDOW('Caption'),AT(,,361,210),GRAY,FONT('Segoe UI',9),RESIZE
>                                 ENTRY(@s20),AT(34,56),USE(?ENTRY1)
>                                 BUTTON('Button1'),AT(140,55),USE(?BUTTON1)
>                                 BUTTON('Close'),AT(304,182,46),USE(?bClose),STD(STD:Close)
>                               END
> im                            TIdleMonitor
> ss                            TScreenSaverBase
>   CODE
>   OPEN(Window)
>   im.Init(Window, 5, ss)
>   ACCEPT
>   END

In other words, you should declare 2 variables: im (TIdleMonitor) and ss (TScreenSaverBase), and call im.Init() somewhere after OPNE(Window).

## Requirements
- Windows 2000 and higher
- C6 and higher, ABC/Legacy
- source code only

## Dependencies
- No

## Price
- $100 [PayPal]([https://www.paypal.me/mikeduglas?ppid=PPC000628&cnac=RU&rsta=ru_RU(ru_RU)&cust=8W29QJ6GKY9HS&unptid=75f96da6-24a4-11e9-ae2c-441ea14e9560&t=&cal=ff0291196b3f5&calc=ff0291196b3f5&calf=ff0291196b3f5&unp_tpcid=ppme-social-user-profile-created&page=main:email&pgrp=main:email&e=op&mchn=em&s=ci&mail=sys])