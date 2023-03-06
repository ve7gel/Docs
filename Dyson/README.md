# udi-poly-dysonfan
UDI Poly for Dyson TP series fans. I only have a TP07 DysonPureCool so haven't tested it with any other models.  There
is currently no support for any heat models.  If you are interested in adding support and are willing to test, PM me on 
the UDI Forum (@glarsen). 

This nodeserver uses the libdyson Python library by Xiaonan Shen. 

WARNING:  Dyson could change their API at any time 
rendering this nodeserver inoperable.  I can offer no assurances that this can be fixed.

Dyson PH02 PureHumidifyCool support is basic.  Humidity settings are not yet implemented.
Dyson TP02 PureCoolLink support is in BETA.  Please report any issues on the forum.

Configuration will require downloading https://github.com/shenxn/libdyson/blob/main/get_devices.py from libdyson, and 
then running it "python3 get_devices.py".  Supply your account email address and password, then enter the token that you
receive at the email address registered on your account.  The program will the supply the credential.  Copy and save it.

###Version History:

4.0.1 January 25, 2023
- move version info from server.json

4.0.0 January 19, 2023
- release - add support for PureCoolHumidity series 358, 358E, 358K.  Thanks to UDI Forum member jwagner10 for his assistance in testing the code on the 358k

3.3.1 April 29, 2022
- add BETA support for TP02 (model 475)

3.2.1 April 21, 2022
- add some config error trapping and messages at startup

3.2.0 March 10, 2022
- change uom for ppm to ug/m3 to display ppm correctly in UI
- add humidity settings for PH02

3.1.5, 3.1.6 February 28, 2022
- bug fix for PH02

3.1.4 February 28, 2022
- fix fan status display. Change how auto mode and fan speed display in UI

3.1.2, 3.1.3 February 26, 2022
- added basic support for PureCoolHumidify
- fixed F/C units display

3.1.1 February 24, 2022
- working on support for PureCoolHumidify

3.1.0 February 21, 2022
- add support for oscillation angle control

3.0.6 February 16, 2022
- code formatting and fix won't install from store

3.0.5 January 15, 2022
- add support for continuous monitoring enable/disable

3.0.4 January 12, 2022
- Minor code changes to fix first startup after configuration

3.0.3 January 12, 2022
- Update profile to correct units for particulates, VOCs and NOx

3.0.2 January 12, 2022
- Minor code changes

3.0.2 January 11, 2022
- Add support for airflow direction control

3.0.1 January 11, 2022
- Add support for F or C temperature display.  Library seems to always report temperature in degress Kelvin,
  so conversion should always be same regardless of model or country.
- Add support for switching power off and on

3.0.0 January 10, 2022
- Initial release for PG3