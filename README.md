# mCerebrum-Configuration

mCerebrum is a configurable smartphone software platform for mobile and wearable sensors. It provides support for reliable data collection from mobile and wearable sensors, and offers real-time processing of these data.

This repo contains configurations for mCerebrum studies.

You can find more information about MD2K software on our [software website](https://md2k.org/software) or the MD2K organization on our [MD2K website](https://md2k.org/).


##### Scheduler
| Name | Default Config| Config|Description
|---|---|---|---|
|`core_id` | &#9745; |
|`core_enable` | &#9745;|&#9745;|

<br>Schedule</br>


| Field |required|Description|Example
|---|---|---|---|
|`id` | &#9745;| unique id for this scheduler|`"id": "wakeup"`
|`observe[]` || list of events to observe<br><br>Events:<br>1) DataSource<br>2) DateTime<br>3) Time| `"observe":[`<br>`"WAKEUP-----",`<br>`"00:00:00`<br>`]`|
|`startIf`||Conditional statement to start scheduling (if it's not running)|
|`stopIf`||Conditional statement to stop scheduling defines whether it's possible to schedule|
|`startTime`|||
|`endTime`|||
|`recurrence`|||


<br> Trigger When

| Field |required|Description|Example
|---|---|---|---|
|`id` | &#9745;| unique id for this scheduler|`"id": "wakeup"`
|`observe[]` || list of events to observe<br><br>Events:<br>1) DataSource<br>2) DateTime<br>3) Time| `"observe":[`<br>`"WAKEUP-----",`<br>`"00:00:00`<br>`]`|
|`startIf`||Conditional statement to start scheduling (if it's not running)|
|`stopIf`||Conditional statement to stop scheduling defines whether it's possible to schedule|
|`startTime`|||
|`endTime`|||
|`recurrence`|||


##### Core
| Name | Default Config| Config|Description
|---|---|---|---|
|`core_id` | &#9745; |
|`core_enable` | &#9745;|&#9745;|

##### Config Info

| Name | Default Config| Config|Description
|---|---|---|---|
|`core_config_id` | &#9745; |
|`core_config_title` | &#9745;|
|`core_config_description` | &#9745;|
|`core_config_version` | &#9745;|
|`core_config_filename` |&#9745; |&#9745;|
|`core_config_from` |  |&#9745;|local, cerebral_cortex
|`core_config_createTime`||&#9745;|
|`core_config_icon`<br> ` - name`<br>` - type`<br>` - content`|&#9745;||
##### Login
| Name | Default Config| Config|Description
|---|---|---|---|
|`core_login_serverAddress` | &#9745; |&#9745;|Example: `https://odin.md2k.org`|
|`core_login_isLoggedIn`| | &#9745;|
|`core_login_username`| | &#9745;|
|`core_login_password`| | &#9745;|
|`core_login_accessToken`| | &#9745;|

##### privacy
| Name | Default Config| Config|Description
|---|---|---|---|
|`core_privacy_durationChoices`<br>`- id`<br>`- title`<br>`- timestamp` | &#9745; ||
|`core_privacy_dataSourceChoices`<br>`- id`<br>`- title`<br>`- dataSources` | &#9745; ||

##### upload
| Name | Default Config| Config|Description
|---|---|---|---|
|`core_upload_enable`||&#9745;|
|`core_upload_rules`<br>`- id`<br>`- enable`<br>`- title`<br>`- interval`<br>`- condition`<br>`- includeDataSources`<br>`- excludeDataSources` | &#9745; ||

##### PhoneSensor
| Name | Values| Default Value|Description
|---|---|---|---|
|`phonesensor_accelerometer_enable`|`true/false`|`false` |
|`phonesensor_accelerometer_sampleRate`| `1-100`|`16` |&#9745;|
|`phonesensor_accelerometer_sampleRateUnit`| `SECOND`|`SECOND` |&#9745;|
|`phonesensor_accelerometer_writeType`|`FIXED/AS_RECEIVED/ON_CHANGE`| `FIXED` ||
|`phonesensor_accelerometerLinear_enable`| &#9745; |&#9745;|
|`phonesensor_accelerometerLinear_sampleRate`| &#9745; |&#9745;|
|`phonesensor_accelerometerLinear_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_accelerometerLinear_writeType`| &#9745; |&#9745;|
|`phonesensor_gyroscope_enable`| &#9745; |&#9745;|
|`phonesensor_gyroscope_sampleRate`| &#9745; |&#9745;|
|`phonesensor_gyroscope_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_gyroscope_writeType`| &#9745; |&#9745;|
|`phonesensor_magnetometer_enable`| &#9745; |&#9745;|
|`phonesensor_magnetometer_sampleRate`| &#9745; |&#9745;|
|`phonesensor_magnetometer_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_magnetometer_writeType`| &#9745; |&#9745;|
|`phonesensor_gravity_enable`| &#9745; |&#9745;|
|`phonesensor_gravity_sampleRate`| &#9745; |&#9745;|
|`phonesensor_gravity_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_gravity_writeType` | &#9745; |&#9745;|
|`phonesensor_ambientLight_enable`| &#9745; |&#9745;|
|`phonesensor_ambientLight_sampleRate`| &#9745; |&#9745;|
|`phonesensor_ambientLight_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_ambientLight_writeType`| &#9745; |&#9745;|
|`phonesensor_airPressure_enable`| &#9745; |&#9745;|
|`phonesensor_airPressure_sampleRate`| &#9745; |&#9745;|
|`phonesensor_airPressure_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_airPressure_writeType`| &#9745; |&#9745;|
|`phonesensor_ambientTemperature_enable`| &#9745; |&#9745;|
|`phonesensor_ambientTemperature_sampleRate`| &#9745; |&#9745;|
|`phonesensor_ambientTemperature_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_ambientTemperature_writeType` | &#9745; |&#9745;|
|`phonesensor_proximity_enable`| &#9745; |&#9745;|
|`phonesensor_proximity_sampleRate`| &#9745; |&#9745;|
|`phonesensor_proximity_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_proximity_writeType`| &#9745; |&#9745;|
|`phonesensor_relativeHumidity_enable`| &#9745; |&#9745;|
|`phonesensor_relativeHumidity_sampleRate`| &#9745; |&#9745;|
|`phonesensor_relativeHumidity_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_relativeHumidity_writeType`| &#9745; |&#9745;|
|`phonesensor_significantMotion_enable`| &#9745; |&#9745;|
|`phonesensor_significantMotion_writeType`| &#9745; |&#9745;|
|`phonesensor_chargingStatus_enable`| &#9745; |&#9745;|
|`phonesensor_chargingStatus_sampleRate`| &#9745; |&#9745;|
|`phonesensor_chargingStatus_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_chargingStatus_writeType`| &#9745; |&#9745;|
|`phonesensor_bluetoothStatus_enable`| &#9745; |&#9745;|
|`phonesensor_bluetoothStatus_sampleRate`| &#9745; |&#9745;|
|`phonesensor_bluetoothStatus_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_bluetoothStatus_writeType`| &#9745; |&#9745;|
|`phonesensor_gpsStatus_enable`| &#9745; |&#9745;|
|`phonesensor_gpsStatus_sampleRate`| &#9745; |&#9745;|
|`phonesensor_gpsStatus_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_gpsStatus_writeType`| &#9745; |&#9745;|
|`phonesensor_wifiStatus_enable`| &#9745; |&#9745;|
|`phonesensor_wifiStatus_sampleRate`| &#9745; |&#9745;|
|`phonesensor_wifiStatus_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_wifiStatus_writeType`| &#9745; |&#9745;|
|`phonesensor_battery_enable`| &#9745; |&#9745;|
|`phonesensor_battery_sampleRate`| &#9745; |&#9745;|
|`phonesensor_battery_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_battery_writeType`| &#9745; |&#9745;|
|`phonesensor_activityType_enable`| &#9745; |&#9745;|
|`phonesensor_activityType_sampleRate`| &#9745; |&#9745;|
|`phonesensor_activityType_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_activityType_writeType`| &#9745; |&#9745;|
|`phonesensor_gps_enable`| &#9745; |&#9745;|
|`phonesensor_gps_sampleRate`| &#9745; |&#9745;|
|`phonesensor_gps_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_gps_writeType`| &#9745; |&#9745;|

##### MotionSense
|Varialble |Default Config| Config|Description
|---|:---:|:---:|-----|
|`motionsense_requiredDevice`<br>`- RequiredDevice[]`| &#9745; ||
|`motionsense_runAsForegroundService`| &#9745; |&#9745;|
|`motionsense_deviceSettings`<br> `- DeviceSettings[]`| &#9745; |&#9745;||
|`motionsense_devices[Device]`| &#9745; |&#9745;||
##### RequiredDevice
| Variable| Default Config| Config|Description|
|---|---|---|---|
|`motionsense_device_platformType`| &#9745; ||
|`motionsense_device_platformId`| &#9745; |&#9745;|
|`motionsense_device_version`|&#9745;||
|`motionsense_device_required`|&#9745;||
##### DeviceSettings
| Variable| Default Config| Config|Description|Supported devices|
|---|---|---|---|-----|
|`motionsense_device_platformType`| &#9745; |||MotionSense, MotionSenseHRV|
|`motionsense_device_platformId`| &#9745; |&#9745;||MotionSense, MotionSenseHRV|
|`motionsense_device_version`|&#9745;|||MotionSense, MotionSenseHRV|
|`motionsense_device_minimumConnectionInterval`| &#9745; |&#9745;|
|`motionsense_accelerometer_enable`| &#9745; |&#9745;||MotionSense, MotionSenseHRV, MotionSenseHRV+, MotionSenseHRV+Gen2|
|`motionsense_accelerometer_frequency`| &#9745; |&#9745;||MotionSense, MotionSenseHRV, MotionSenseHRV+, MotionSenseHRV+Gen2|
|`motionsense_accelerometer_sensitivity`| &#9745; |&#9745;||MotionSenseHRV+Gen2|
|`motionsense_gyroscope_enable`| &#9745; |&#9745;||MotionSense, MotionSenseHRV|
|`motionsense_gyroscope_frequency`| &#9745; |&#9745;||MotionSense, MotionSenseHRV|
|`motionsense_gyroscope_sensitivity`| &#9745; |&#9745;||MotionSenseHRV+Gen2|
|`motionsense_sequenceNumberMotion_enable`| &#9745; |&#9745;||MotionSense, MotionSenseHRV, MotionSenseHRV+|
|`motionsense_sequenceNumberMotion_frequency`| &#9745; |&#9745;||MotionSense, MotionSenseHRV, MotionSenseHRV+|
|`motionsense_rawMotion_enable`| &#9745; |&#9745;||MotionSense, MotionSenseHRV, MotionSenseHRV+|
|`motionsense_rawMotion_frequency`| &#9745; |&#9745;||MotionSense, MotionSenseHRV, MotionSenseHRV+|
|`motionsense_battery_enable`| &#9745; |&#9745;||MotionSense, MotionSenseHRV, MotionSenseHRV+|
|`motionsense_led_enable`| &#9745; |&#9745;||MotionSenseHRV, MotionSenseHRV+|
|`motionsense_led_frequency`| &#9745; |&#9745;||MotionSenseHRV, MotionSenseHRV+|
|`motionsense_led_filteredEnable`| &#9745; |&#9745;||MotionSenseHRV+Gen2|
|`motionsense_led_red`| &#9745; |&#9745;||MotionSenseHRV+Gen2|
|`motionsense_led_green`| &#9745; |&#9745;||MotionSenseHRV+Gen2|
|`motionsense_led_infrared`| &#9745; |&#9745;||MotionSenseHRV+Gen2|
|`motionsense_rawLed_enable`| &#9745; |&#9745;||MotionSenseHRV+Gen2|
|`motionsense_quaternion_enable`| &#9745; |&#9745;||MotionSenseHRV+|
|`motionsense_quaternion_frequency`| &#9745; |&#9745;||MotionSenseHRV+|
|`motionsense_magnetometer_enable`| &#9745; |&#9745;||MotionSenseHRV+|
|`motionsense_magnetometer_frequency`| &#9745; |&#9745;||MotionSenseHRV+|
|`motionsense_magnetometerSensitivity_enable`| &#9745; |&#9745;||MotionSenseHRV+|
|`motionsense_magnetometerSensitivity_frequency`| &#9745; |&#9745;||MotionSenseHRV+|
|`motionsense_rawMagnetometer_enable`| &#9745; |&#9745;||MotionSenseHRV+|
|`motionsense_rawMagnetometer_frequency`| &#9745; |&#9745;||MotionSenseHRV+|
|`motionsense_sequenceNumberMagnetometer_enable`| &#9745; |&#9745;||MotionSenseHRV+|
|`motionsense_sequenceNumberMagnetometer_frequency`| &#9745; |&#9745;||MotionSenseHRV+|


##### Device
| Variable| Default Config| Config|Description|Device
|---|---|---|---|-----|
|`motionsense_device_id`|&#9745;|||MotionSense, MotionSenseHRV|
|`motionsense_device_enable`| &#9745; |||MotionSense, MotionSenseHRV|
|`motionsense_device_platformType`| &#9745; |||MotionSense, MotionSenseHRV|
|`motionsense_device_platformId`| &#9745; |&#9745;||MotionSense, MotionSenseHRV|
|`motionsense_device_version`|&#9745;|||MotionSense, MotionSenseHRV|



## Contributing
Please read our [Contributing Guidelines](https://md2k.org/software/under-the-hood/contributing) for details on the process for submitting pull requests to us.

We use the [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html).

Our [Code of Conduct](https://md2k.org/software/CodeofConduct) is the [Contributor Covenant](https://www.contributor-covenant.org/).

Bug reports can be submitted through [JIRA](https://md2korg.atlassian.net/secure/Dashboard.jspa).

Our discussion forum can be found [here](https://discuss.md2k.org/).

## Versioning

We use [Semantic Versioning](https://semver.org/) for versioning the software which is based on the following guidelines.

MAJOR.MINOR.PATCH (example: 3.0.12)

  1. MAJOR version when incompatible API changes are made,
  2. MINOR version when functionality is added in a backwards-compatible manner, and
  3. PATCH version when backwards-compatible bug fixes are introduced.

For the versions available, see [this repository's tags](https://github.com/MD2Korg/mCerebrum-Configuration/tags).

## Contributors

Link to the [list of contributors](https://github.com/MD2Korg/mCerebrum-Configuration/graphs/contributors) who participated in this project.

## License

This project is licensed under the BSD 2-Clause - see the [license](https://md2k.org/software-under-the-hood/software-uth-license) file for details.

## Acknowledgments

* [National Institutes of Health](https://www.nih.gov/) - [Big Data to Knowledge Initiative](https://datascience.nih.gov/bd2k)
  * Grants: R01MD010362, 1UG1DA04030901, 1U54EB020404, 1R01CA190329, 1R01DE02524, R00MD010468, 3UH2DA041713, 10555SC
* [National Science Foundation](https://www.nsf.gov/)
  * Grants: 1640813, 1722646
* [Intelligence Advanced Research Projects Activity](https://www.iarpa.gov/)
  * Contract: 2017-17042800006
