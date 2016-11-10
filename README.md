Hello-OBP-OAuth1.0a-Android
========================

This is a basic app to demonstrate the integration of the OpenBankProject
with OAuth1.0-Authentication into an Android application. 
The app will run through OAuth authentication, and then make an OAuth signed API request
that retrieves the list of banks available on the sandbox API.
Though this particular API call does not require OAuth,
this project uses OAuth to do so anyways, in order to demonstrate the process.


## SETUP

There are a couple of things you need to do to get this project set up.

Get consumer key / secret:  
- Register your client at https://apisandbox.openbankproject.com/consumer-registration
- Set `OBP_AUTH_KEY` and `OBP_SECRET_KEY` in `OBPRestClient.java` file.
- Change customAppProtocol in `res/values/strings.xml` (Not strictly required, but recommended.)
- Change the package name of the app (Not strictly required, but recommended. This might be a step you take after getting it running.)
- Remove the `RuntimeException` in `OAuthActivity.java` that is there to remind you of these steps/


## Login credentials

You will need to login to the OBP Sandbox API (unless you change the API instance) when running the app.

This can be done using any the following credentials:

```
username: joe.bloggs@example.com
password: qwerty

username: jane.bloggs@example.com
password: qwerty

username: john.bloggs@example.com
password: qwerty
```


## LICENSE

This project is licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
