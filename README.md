Hello-OBP-OAuth1.0a-Android
========================

This is a basic app to demonstrate the integration of the OpenBankProject with OAuth1.0-Authentication into an Android application. 
The app will run through OAuth authentication, and then make an OAuth signed API request that retrieves the list of banks available
on the sandbox API. Though this particular API call does not require OAuth, this project uses OAuth to do so anyways, in order to 
demonstrate the process.

## SETUP

There are a couple of things you need to do to get this project set up.

Get consumer key / secret:  
-register your client at  https://apisandbox.openbankproject.com/consumer-registration

-set OBP_AUTH_KEY and OBP_SECRET_KEY in OBPRestClient.java

Change customAppProtocol in res/values/strings.xml (Not strictly required, but recommended)
Change the package name of the app (Not strictly required, but recommended. This might be a step you take after getting it running.)

Remove the RuntimeException in OAuthActivity.java that is there to remind you of these steps/

## Login credentials

You will need to login to the OBP Sandbox API (unless you change the API instance) when running the app. 

Please see the wiki page of each sandbox for credentials.


## LICENSE

This project is licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
