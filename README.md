# AospExtended OS
## Official builds application

Before opening a pull request to add your build into our official website, you should know a few simple things:

### 1. Hosting

Our files are hosted on [SourceForge](https://sourceforge.net/projects/aospextended-rom/)

### 2. Changelog
For each new version, you need to upload the changelog to this repository in the device specific folder.

The changelog file name must match the **.zip** file name and should end with **.txt**
Eg: **.zip** is **AospExtended-v6.2-osprey-20180906-0543-OFFICIAL.zip**, changelog file name should be **AospExtended-v6.2-osprey-20180906-0543-OFFICIAL.txt**

### 3. Addons
You can add links to device specific addons(firmwares patches, tweaks, hotfixes etc) in [addons.json](https://github.com/AospExtended-Devices/official_builds/blob/master/addons.json) , it will appear inside OTA app. Make sure to follow the syntax and
avoid adding duplicate addons that already exists in **default** array, those are universal addons that can be used on all the devices.

### 4. Over-the-air (OTA) updates
Our system is automatic, you should not worry about updating some script, just upload the new build to the [SourceForge](https://sourceforge.net/projects/aospextended-rom/) and send a pull request with the changelog and also edit your device JSON file (**builds/your_device_codename.json**) in this repository.

Eg: Moto G 2015 is called **osprey**, so the device JSON file is **builds/osprey.json**

**Note:** New builds can take up to 30 minutes to appear on the site and in the OTA application.

### 5. JSON parameters
| Param | Description | Required |
|--|--|--|
| oreo/pie | Version name, will be shown on download portal | Yes |
| file_name | Latest build name | Yes |

Example: [Click here](https://github.com/AospExtended-Devices/official_builds/blob/master/builds/kenzo.json)

**Please format your JSON code properly, [here](https://jsonformatter.curiousconcept.com/).**

### 6. Build type
You need to add 'export EXTENDED_BUILD_TYPE=OFFICIAL' in your build environment so that the OTA app will be included in your build.

### 7. Device tree
Maintainers should upload their device trees on https://github.com/AospExtended-Devices

### Important Links:

- [Website](http://www.aospextended.com/)
- [Download Center](https://downloads.aospextended.com/)
- [Blog](https://blog.aospextended.com/)
- [Gerrit Code Review](http://gerrit.aospextended.com/)
- [Apply for Official Device](https://github.com/AospExtended/Documentation_and_thread-template)
- [Telegram Channel](https://telegram.me/aospextended/)
- [Documentation, Official Devices & Thread Template](https://github.com/AospExtended/Documentation_and_thread-template/) 
- [Help us translate AospExtended ROM and bring it to the world!](http://translate.aospextended.com/)
- [Theme Resources](https://github.com/AospExtended/AEX-Scripts/) 
- [Extended Devices](https://github.com/AospExtended-devices/)
- [Gallery](https://aospextended.com/gallery)
- [Facebook page!](https://www.facebook.com/aospextended/)
