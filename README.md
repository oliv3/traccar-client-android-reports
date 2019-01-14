# Traccar Android client reports

This repository aims to help fixing the [Traccar Android client](https://github.com/traccar/traccar-client-android).

Since version 5.12, sending location updates to [Traccar](https://traccar.org) server has become unstable, changing
regularly (5.17 is the current version), and definitely not improving,
to a point where using only GPS and setting the client to maximum accuracy is the only way to get it reporting.

There are numerous open [issues](https://github.com/traccar/traccar-client-android/issues):
* [#390](https://github.com/traccar/traccar-client-android/issues/390)
* [#367](https://github.com/traccar/traccar-client-android/issues/367)
* And [more](https://github.com/traccar/traccar-client-android/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aopen+location)...

# What you can do

Clone this repository and report how functional your client is:

* Android version
* Phone brand/model
* Traccar version and flavor
* for different phone and application settings

## Where to put reports

We'll use a directory-based structure:

`[VERSION]/[OS]/[BRAND]/[MODEL]/README.md`

Where:

* `[VERSION]` is the client version
* `[OS]` is the android version
* `[BRAND]` and `[MODEL]` for the phone

e.g: `5.17/8.0.0/Sony/F5321/README.md`

## Report

The following report should be generic enough to suit most of Android phones.

Fill the report with your details, and for the tests you've done, report if the
application is:

* sending location updates (:heavy_check_mark:)
* or not (:x:).

Copy this [sample](https://github.com/oliv3/traccar-client-android-reports/tree/wip/5.17/8.0.0/Sony/F5321) README.md in your directory:

=[ CUT HERE ]===================================================================

```
**Brand / model**: Sony / Xperia X Compact

**OS**: Android / 8.0.0

**Client**: 5.17

**Flavor**:
 - [x] Google Play store
 - [ ] F-Droid
 - [ ] Other APK:

**Phone settings**:
1. **H**igh accuracy: GPS, mobile network, Wi-Fi and Bluetooth
2. **B**attery saving: Mobile network, Wi-Fi and Bluetooth
3. **G**PS only (one can expect the same results as 1.)

**Traccar settings**:
1. **H**igh
2. **M**edium
3. **L**ow

**Results**:

&nbsp; | High | Medium | Low
-:|:-:|:-:|:-:
Phone: **H**igh accuracy | :heavy_check_mark: | :x: | :heavy_check_mark:
**B**attery saving | :x: | :x: | :x:
**G**PS only | :heavy_check_mark: | :x: | :heavy_check_mark:

**Additional notes**:

Tests were run in the open-air, device in motion with settings:

* Update frequency: 1s
* Minimal distance: 0
* Minimal angle: 0
```

=[ REPORT ]=====================================================================

**Brand / model**: Sony / Xperia X Compact

**OS**: Android / 8.0.0

**Client**: 5.17

**Flavor**:
 - [x] Google Play store
 - [ ] F-Droid
 - [ ] Other APK:

**Phone settings**:
1. **H**igh accuracy: GPS, mobile network, Wi-Fi and Bluetooth
2. **B**attery saving: Mobile network, Wi-Fi and Bluetooth
3. **G**PS only (one can expect the same results as 1.)

**Traccar settings**:
1. **H**igh
2. **M**edium
3. **L**ow

**Results**:

&nbsp; | High | Medium | Low
-:|:-:|:-:|:-:
Phone: **H**igh accuracy | :heavy_check_mark: | :x: | :heavy_check_mark:
**B**attery saving | :x: | :x: | :x:
**G**PS only | :heavy_check_mark: | :x: | :heavy_check_mark:

**Additional notes**:

Tests were run in the open-air, device in motion with settings:

* Update frequency: 1s
* Minimal distance: 0
* Minimal angle: 0
