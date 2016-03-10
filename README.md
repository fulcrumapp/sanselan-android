[![Build Status](https://travis-ci.org/fulcrumapp/sanselan-android.svg?branch=master)](https://travis-ci.org/fulcrumapp/sanselan-android)

#### Check out [releases](https://github.com/fulcrumapp/sanselan-android/releases) to get the latest jar.

This repository is forked from https://code.google.com/archive/p/sanselanandroid/.

0.97 was the last stable release of [Sanselan](https://commons.apache.org/proper/commons-imaging/download_sanselan.cgi), a library that reads and writes a variety of image formats, including fast parsing of image info (size, color space, ICC profile, etc.) and metadata. Sanselan has since been swallowed up and is now part of [Apache Commons Imaging](https://commons.apache.org/proper/commons-imaging/).

It is necessary to maintain `sanselan-android` because there are modifications and re-definitions necessary to enable Sanselan to work correctly on Android (plug: [read our post](http://www.fulcrumapp.com/blog/adding-photo-quality-settings-on-android/)). Additionally, there isn't currently a stable release of Apache Commons Imaging (especially one with the aforementioned tweaks).

## Building

If you need to make modifications, you should submit a PR! but if we're too slow ... ... ... and you need to make changes/get your own jar, check out the repo and:

1) upgrade the `version` in `build.gradle`

2) then in the root run:

    ./gradlew clean build

This will create a new jar in `build/libs`.

