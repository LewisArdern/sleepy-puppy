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
* Fix issue with 'Repeater' adding + instead of URL encode, breaking payloads e.g ```"><img+src%3d'//buildingsecurity.in/mH'/>```

# Build Steps:

1. Install Gradle
2. Run ```gradle clean jar```
3. Outputs to ```/build/libs/wokepuppy-burp.jar```



## Original Work && Authors: 

* [Page](https://github.com/netflix/sleepy-puppy)
* [API Documentation](https://github.com/netflix/sleepy-puppy/wiki/API)
* [Scott Behrens](https://github.com/sbehrens) & [Patrick Kelley](https://github.com/monkeysecurity) for developing the awesome Sleepy Puppy and its API documentation
