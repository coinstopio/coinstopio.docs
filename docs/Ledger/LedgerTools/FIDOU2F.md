
# FIDO U2F

FIDO U2F is a two-factor authentication method (2FA) developed by the [FIDO Alliance](https://fidoalliance.org/) that is supported on the Ledger Nano S and Ledger Blue devices. It works with several web services, like Facebook, Dashlane, Gmail, Dropbox, GitHub, etc.

-   FIDO U2F increases your account security as both your password **and** **Ledger device** are required to login.
-   FIDO U2F is not related to cryptocurrencies. It's an additional utility for your Ledger device.

## Prerequisites

-   A Ledger Nano S or Ledger Blue with the latest firmware version.
-   Ledger Live should be [downloaded](https://www.ledger.com/pages/ledger-live) and installed.

## Instructions

Set up FIDO U2F

1.  Open the **Manager** in Ledger Live.
2.  Connect and unlock your Ledger device.
3.  If asked, allow the manager on your device by pressing the right button.
4.  Find **FIDO U2F** in the app catalog.
5.  Click the **Install** button of the app.
    -   An installation window appears.
    -   Your device will display **Processing...**
    -   The app installation is confirmed.
6.  Open FIDO U2F from the dashboard of your device.
7.  Go to the security parameters of web services partnering with FIDO U2F and follow their instructions to register your device: [Facebook](https://www.facebook.com/help/401566786855239), [Dashlane](https://support.dashlane.com/hc/en-us/articles/202625042-Protect-your-account-using-Two-Factor-Authentication#title3), [Google](https://myaccount.google.com/signinoptions/two-step-verification/enroll-welcome), [GitHub](https://help.github.com/articles/configuring-two-factor-authentication-via-fido-u2f/), [Dropbox](https://www.dropbox.com/fr/help/363).

Always ensure you set up an alternative login method. Reinstalling FIDO U2F requires you reconfigure it for each service.

Restore FIDO U2F after a firmware update

The FIDO U2F app on your Ledger device maintains an internal counter that changes each time you use FIDO U2F to login on a third party service. After a firmware update, all apps have to be reinstalled. Unfortunately, this means that the counter is reset and you will not be able to login using the FIDO U2F app on your device before reconfiguring the services you use it on:

1.  Please use an alternative means of logging in onto the services you want to access (_authenticator app / one time password / request a password reset link by email_).
2.  Once logged in, go into the (security) settings of the services on which you use FIDO U2F. Then, remove FIDO U2F with your Ledger device as a method of authentication.
3.  Re-register your device as authentication method.