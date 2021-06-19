# CrashingApp
Sample to show difference in UnHandledException handling between UWP and WinUI3

This repo contains 2 'identical' projects. Both show a button that will crash the app (divide-by-zero) from a background Task.
Both apps don't handle the exception locally. 
The UWP app is able to catch the exception at App level (App_UnhandledException), while the WinUI3 is not able to catch the error in the App_UnhandledException and therefore unable to do some last-resort work (eg., sending Crash report to AppService).
