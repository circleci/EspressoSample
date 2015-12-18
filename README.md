# CircleCI Espresso sample

Highlights:

* `com.android.ddmlib.DdmPreferences.setTimeOut(60000)` in the
  `android.defaultConfig` section of the `build.gradle` file
  ([example](https://github.com/circleci/EspressoSample/blob/master/app/build.gradle))

* the `circle.yml` sets the ADB_INSTALL_TIMEOUT environment variable
  ([example](https://github.com/circleci/EspressoSample/blob/master/circle.yml#L5))

* there is a `sleep 30` command before the screen unlock operation
  ([example](https://github.com/circleci/EspressoSample/blob/master/circle.yml#L22))

We also recommend that you set the `TERM` variable to `dumb` for better
Gradle command-line output
([example](https://github.com/circleci/EspressoSample/blob/master/circle.yml#L4)).
