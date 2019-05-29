# mCerebrum-Configuration

mCerebrum is a configurable smartphone software platform for mobile and wearable sensors. It provides support for reliable data collection from mobile and wearable sensors, and offers real-time processing of these data.

This repo contains configurations for mCerebrum studies.

You can find more information about MD2K software on our [software website](https://md2k.org/software) or the MD2K organization on our [MD2K website](https://md2k.org/).

#### Variables:

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
|`core_config_filename` | |&#9745;|
|`core_config_from` |  |&#9745;|local, cerebral_cortex
|`core_config_createTime`||&#9745;|
|`core_config_icon[name,type,content]`|&#9745;||
##### Login
| Name | Default Config| Config|Description
|---|---|---|---|
|`core_login_serverAddress` | &#9745; |&#9745;|Example: `https://odin.md2k.org`|
|`core_login_isLoggedIn` | &#9745;|
|`core_login_username`| | &#9745;|
|`core_login_password`| | &#9745;|
|`core_login_accessToken`| | &#9745;|

##### privacy
| Name | Default Config| Config|Description
|---|---|---|---|
|`core_privacy_durationChoices[id,title,timestamp]` | &#9745; ||
|`core_privacy_dataSourceChoices[id,title,dataSources]` | &#9745; ||

##### upload
| Name | Default Config| Config|Description
|---|---|---|---|
|`core_upload_enable`||&#9745;|
|`core_upload_rules[id,enable,title,interval,condition,includeDataSources,excludeDataSources]` | &#9745; ||

##### PhoneSensor
| Name | Default Config| Config|Description
|---|---|---|---|
|`phonesensor_accelerometer_enable`| &#9745; |&#9745;|
|`phonesensor_accelerometer_sampleRate`| &#9745; |&#9745;|
|`phonesensor_accelerometer_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_accelerometer_writeType`| &#9745; |&#9745;|
|`phonesensor_accelerometer_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_accelerometer_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_accelerometerLinear_enable`| &#9745; |&#9745;|
|`phonesensor_accelerometerLinear_sampleRate`| &#9745; |&#9745;|
|`phonesensor_accelerometerLinear_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_accelerometerLinear_writeType`| &#9745; |&#9745;|
|`phonesensor_accelerometerLinear_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_accelerometerLinear_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_gyroscope_enable`| &#9745; |&#9745;|
|`phonesensor_gyroscope_sampleRate`| &#9745; |&#9745;|
|`phonesensor_gyroscope_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_gyroscope_writeType`| &#9745; |&#9745;|
|`phonesensor_gyroscope_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_gyroscope_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_magnetometer_enable`| &#9745; |&#9745;|
|`phonesensor_magnetometer_sampleRate`| &#9745; |&#9745;|
|`phonesensor_magnetometer_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_magnetometer_writeType`| &#9745; |&#9745;|
|`phonesensor_magnetometer_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_magnetometer_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_gravity_enable`| &#9745; |&#9745;|
|`phonesensor_gravity_sampleRate`| &#9745; |&#9745;|
|`phonesensor_gravity_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_gravity_writeType` | &#9745; |&#9745;|
|`phonesensor_gravity_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_gravity_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_ambientLight_enable`| &#9745; |&#9745;|
|`phonesensor_ambientLight_sampleRate`| &#9745; |&#9745;|
|`phonesensor_ambientLight_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_ambientLight_writeType`| &#9745; |&#9745;|
|`phonesensor_ambientLight_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_ambientLight_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_airPressure_enable`| &#9745; |&#9745;|
|`phonesensor_airPressure_sampleRate`| &#9745; |&#9745;|
|`phonesensor_airPressure_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_airPressure_writeType`| &#9745; |&#9745;|
|`phonesensor_airPressure_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_airPressure_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_ambientTemperature_enable`| &#9745; |&#9745;|
|`phonesensor_ambientTemperature_sampleRate`| &#9745; |&#9745;|
|`phonesensor_ambientTemperature_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_ambientTemperature_writeType` | &#9745; |&#9745;|
|`phonesensor_ambientTemperature_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_ambientTemperature_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_proximity_enable`| &#9745; |&#9745;|
|`phonesensor_proximity_sampleRate`| &#9745; |&#9745;|
|`phonesensor_proximity_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_proximity_writeType`| &#9745; |&#9745;|
|`phonesensor_proximity_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_proximity_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_relativeHumidity_enable`| &#9745; |&#9745;|
|`phonesensor_relativeHumidity_sampleRate`| &#9745; |&#9745;|
|`phonesensor_relativeHumidity_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_relativeHumidity_writeType`| &#9745; |&#9745;|
|`phonesensor_relativeHumidity_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_relativeHumidity_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_significantMotion_enable`| &#9745; |&#9745;|
|`phonesensor_significantMotion_writeType`| &#9745; |&#9745;|
|`phonesensor_chargingStatus_enable`| &#9745; |&#9745;|
|`phonesensor_chargingStatus_writeType`| &#9745; |&#9745;|
|`phonesensor_chargingStatus_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_bluetoothStatus_enable`| &#9745; |&#9745;|
|`phonesensor_bluetoothStatus_writeType`| &#9745; |&#9745;|
|`phonesensor_bluetoothStatus_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_gpsStatus_enable`| &#9745; |&#9745;|
|`phonesensor_gpsStatus_writeType`| &#9745; |&#9745;|
|`phonesensor_gpsStatus_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_wifiStatus_enable`| &#9745; |&#9745;|
|`phonesensor_wifiStatus_writeType`| &#9745; |&#9745;|
|`phonesensor_wifiStatus_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_battery_enable`| &#9745; |&#9745;|
|`phonesensor_battery_writeType`| &#9745; |&#9745;|
|`phonesensor_battery_sampleRate`| &#9745; |&#9745;|
|`phonesensor_battery_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_battery_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_battery_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_activityType_enable`| &#9745; |&#9745;|
|`phonesensor_activityType_sampleRate`| &#9745; |&#9745;|
|`phonesensor_activityType_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_activityType_writeType`| &#9745; |&#9745;|
|`phonesensor_activityType_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_activity_type_writeOnChangeValue`| &#9745; |&#9745;|
|`phonesensor_gps_enable`| &#9745; |&#9745;|
|`phonesensor_gps_sampleRate`| &#9745; |&#9745;|
|`phonesensor_gps_sampleRateUnit`| &#9745; |&#9745;|
|`phonesensor_gps_writeType`| &#9745; |&#9745;|
|`phonesensor_gps_writeOnChangeType`| &#9745; |&#9745;|
|`phonesensor_gps_writeOnChangeValue`| &#9745; |&#9745;|


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
