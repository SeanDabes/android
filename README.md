# DonkeyOS
This is a slightly customized version of Lineage.


### Downloading the code

To start repo:
`repo init https://github.com/SeanDabes/android.git -b lineage-19.1`

To download the code:
`repo sync -j 10 | grep Fetching`
>If you want to see all the `repo sync` stuff, remove the `grep Fetching` part.


### Building

First, you should download all the proprietary code for your device via adding the source in the `roomservice.xml` file inside the `local_manifests` folder.

Start the building scripts:
`. build/envsetup.sh`

Then, start the build with the command:
`brunch`

In the list, select the option for your device.
>You can build directly for your device with the command `brunch <device_name>`
