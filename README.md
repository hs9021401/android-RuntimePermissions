
Android RuntimePermissions Sample
===================================

This sample shows runtime permissions available in the Android M and above.
It shows how to check and request permissions at runtime and how to declare permissions for M-devices
only.

Introduction
------------

Android M introduced runtime permissions. Applications targeting M and above need to request their
permissions at runtime.
All permissions still need to be declared in the AndroidManifest. However, when accessing APIs that
require a permission, the Activity or Fragment has to verify that the permission has been granted
or request the missing permissions. Permissions are checked through
Activity#requestPermissions(String[], int) and Fragment#requestPermissions(String[], int).
Permission requests are sent through Activity#requestPermissions(String[]), and the response
received in the callback Activity#onRequestPermissionsResult(int, permissions[], int[]).

If an application targets an SDK below M, all permissions are granted at runtime and are available
when the application is running. However, if permissions have been turned off in the system settings
for an application targeting an SDK below M, the API will return empty or no data.

Pre-requisites
--------------

- Android SDK vandroid-MNC
- Android Build Tools v22.0.1
- Android Support Repository

Screenshots
-------------

<img src="screenshots/screenshot-1.png" height="400" alt="Screenshot"/> <img src="screenshots/screenshot-2.png" height="400" alt="Screenshot"/> 

Getting Started
---------------

This sample uses the Gradle build system. To build this project, use the
"gradlew build" command or use "Import Project" in Android Studio.

Support
-------

- Google+ Community: https://plus.google.com/communities/105153134372062985968
- Stack Overflow: http://stackoverflow.com/questions/tagged/android

If you've found an error in this sample, please file an issue:
https://github.com/googlesamples/android-RuntimePermissions

Patches are encouraged, and may be submitted by forking this project and
submitting a pull request through GitHub. Please see CONTRIBUTING.md for more details.

License
-------

Copyright 2014 The Android Open Source Project, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.
