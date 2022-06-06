# DonkeyOS
This is a slightly customized version of Lineage.


## Downloading the code

To start repo:
`repo init https://github.com/SeanDabes/android.git -b lineage-19.1`

To download the code:
`repo sync -j 10 | grep Fetching`
>If you want to see all the `repo sync` stuff, remove the `grep Fetching` part.

Once finished, start the building scripts:
`. build/envsetup.sh`

Download the proprietary code for your device:
`breakfast <device_codename>`
>Change <device_codename> with the one from your device (i.e. kebab, cepheus, etc.)

If there is any error while downloading the proprietary code, you should try downloading from another site, like [TheMuppets](https://github.com/themuppets) and adding the source to the `roomservice.xml` file inside the `.repo/local_manifests` folder.


## Building

Start the building scripts, if you haven't done it already:
`. build/envsetup.sh`

Then, start the build with the command:
`brunch`

In the list, select the option for your device, hit `Enter` and sit for a while.
>You can build directly for your device with the command `brunch <device_name>`
