# TitaniumOS
## Official devices application

Devices repository: https://github.com/Titanium-OS-Devices

Things you must know before getting started:

### 1. Hosting

Our files are hosted on [SourceForge](https://sourceforge.net/projects/TitaniumOS/), you will receive access when you join the team.

### 2. Over-the-air (OTA) updates
Our system is automatic, you should not worry about updating some script, just upload the new build to [SourceForge](https://sourceforge.net/projects/TitaniumOS/) and send a pull request with the changelog and also edit your device JSON file (**builds/your_device_codename.json**) in [this](https://github.com/Titanium-OS-Devices/official_builds) repository. Please read the ReadMe file on that repo.

Eg: Asus Zenfone Max Pro M1 is called **X00T**, so the device JSON file is **builds/X00T.json**

**Note:** New builds can take up to 30 minutes to appear in the OTA application.

### 3. JSON parameters
| Param | Description | Required |
|--|--|--|
| name | Device name | Yes |
| brand | Device manufacturer | Yes |
| codename | Device codename, eg: X00T | Yes |
| version_code | Version code, lowercase, eg: ten | Yes |
| version_name | Version name, will be shown on download portal, eg: Ten | Yes |
| maintainer_name | Your name | Yes |
| maintainer_url | Your personal URL, eg: https://github.com/abhirajsinghofficial/ or https://forum.xda-developers.com/member.php?u=8453543 | No  |
| xda_thread | XDA thread URL, eg: * to be added * | No |

**Please format your JSON code properly, [here](https://jsonformatter.curiousconcept.com/).**

### 4. Build type
You need to add 'export TITANIUM_BUILD_TYPE=OFFICIAL' in your build environment so that the OTA app will be included in your build.

### 5. Device tree
Maintainers should upload their device trees on https://github.com/Titanium-OS-Devices

