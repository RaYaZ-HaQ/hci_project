# hci_project

## How to create a new screen

1. Create a copy of Home.java with a different name.
**Example:** ``Test.java`` (Reason: so we don't rewrite the code for the navigation toolbar)

> **Note:** Don't forget to add this new class file to the AndroidManifest.xml or the app will not include it.
2. Similarly create a copy of home.xml (in the layouts folder) and give it a different name. (This file will contain your user interface)
3. In the class, change ``setContentView(R.layout.home);`` to ``setContentView(R.layout.<new_layout_name>);``
4. Build the UI

## Change the starting activity (for testing purposes only)
In the AndroidManifest, change the line ``<activity android:name=".Login">``to ``<activity android:name=".<your_class_name>">``.

Now, when the app is launched <your_new_activity> will be loaded first instead of the login screen. This is for development and testing purposes only and
transitions will have to be programmed later.
