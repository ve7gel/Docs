# udi-poly-dysonfan
UDI Poly for Dyson TP series fans. I only have a TP07 DysonPureCool so haven't tested it with any other models.  There is currently no support for any heat models.  If you are interested in adding support and are willing to test, PM me on the UDI Forum (@glarsen). 
This nodeserver uses the libdyson Python library by Xiaonan Shen
Configuration will require downloading https://github.com/shenxn/libdyson/blob/main/get_devices.py from libdyson, and then running it "python3 get_devices.py".

Supply your account email address and password, then enter the token that you receive at the email address registered on your account.  The program will the supply the credential.  Copy and save it.

###TODO:
###Add features:
- oscillation angle

###Version History:
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