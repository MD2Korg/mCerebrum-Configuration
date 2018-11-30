# AutoSense

## DataSources
#### List of data sources from AutoSense device

| DataSource Type        | DataSource Id           | Description  | Frequency |
| ------------- |:-------------:| ---| ------: |
| RESPIRATION      |  | Measures the movement of the chest and abdominal wall. | 21.3 Hz|
| ECG      |       |  Records the electrical activity of the heart using electrodes placed over the skin  | 64 Hz |
| ACCELEROMETER |       |    Measures the acceleration of the autosense device | 10.67 Hz |
| BATTERY |       |    Measures the battery level of the device | ? |
| SKIN_TEMPERATURE |       |    DISABLED | 1.28 Hz |
| AMBIENT_TEMPERATURE |      |    DISABLED | 1.28 Hz |
| DATA_QUALITY | RESPIRATION     |    Measures the quality of the respiration data (0:good, 1: not worn/loose, 2: no data)  |0.33 Hz |
| DATA_QUALITY | ECG     |    Measures the quality of the ecg data (0:good, 1: not worn/loose, 2: no data) | 0.33 Hz|
| RESPIRATION_RAW |      |    Raw respiration signal captured by autosense device | 21.67 Hz|
| RESPIRATION_BASELINE |      |    Respiration baseline |21.67 Hz |
| DATA_VARIANCE | RESPIRATION     |    Variance of the respiration data |0.33 Hz |
| DATA_VARIANCE | ECG     |    Variance of the ECG data | 0.33 Hz |

#### Other data sources

| DataSource Type        | DataSource Id           | Description  | Frequency |
| ------------- |:-------------:| -----:| ------: |
| APP_USE      |  | User interaction with the app | ON_CHANGE|
| SYSTEM_LOG      |       |   connectivity,  | ON_CHANGE |

## Configure AutoSense sensors:

#### Sample:
```json
{
  "number_of_device_required": "1",                       // value: integer,      default: null (not required)
  "run_as_foreground_service": "true",          // value: true/false,   default: null (means false)
  "log_app_usage": "true",                      // value: true/false,   default: true
  "log_system_status": "true",                  // value: true/false,   default: false
  "permission_to_edit_configuration": "true",                // value: true/false,   default: true
  "devices": [
    {
      "required": "true",                       // value: true/false    default: false
      "platform_type": "AUTOSENSE_CHEST",       // value: fixed
      "platform_id": "CHEST",                   // value: any string,   default: null (user can define it)
      "device_id": null,                        // value: mac address,  default: null (user will define it)

      "sensors": {
        "sensor_list":"all",            // value: sensorType, id, default: null
        "add_to_list": [
          {
            "datasource_type": "ACCELEROMETER"
          },
          {
            "datasource_type": "ECG"
          }
        ],
        "remove_from_list":[

        ]
      }
    }
  ]
}
```
#### Configuration fields
| Field        | Description           | Default Value  |
| ------------- |:-------------| -----:|
| number_of_device_required      |  | null |
| run_as_foreground_service      | (ANDROID ONLY) Set the background service as foreground      |   "false" |
| log_app_usage | Log user interaction to the app   |    $1 |
|log_system_status| | |
|permission_to_edit_configuration| | |
|devices| | |
#### Configuration fields

| Field        | Description           | Default Value  |
| ------------- |:-------------| -----:|

|required| | |
|| | |
|| | |
