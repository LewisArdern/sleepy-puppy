--------------------WOKE-------------------
============
*September 16th, 2019*

(Currently very hacky)

Netflix deprecated Sleepy Puppy, so this is a fork to use the Burp extension without relying on Sleepy Puppy which can be used for other tools such as XSS Hunter or bXSS.

-Lewis 

# TODO:

* Remove Sleepy Puppy code that isn't necessary
* Update payload generation vs hard-coded
    * Come from a configuration file
    * Default set ability
    * Add custom payloads
    * Until customization parts complete just update parsePayloads in \burp-extension\src\main\java\com\netflix\sleepypuppy\SleepyPuppyConnector.java and rebuild extension

# Build Steps:

1. Install Gradle
2. Run ```gradle clean jar```
3. Outputs to ```/build/libs/wokepuppy-burp.jar```



## Original Work: 

* [Page](https://github.com/netflix)
* [API Documentation](https://github.com/netflix/sleepy-puppy/wiki/API)