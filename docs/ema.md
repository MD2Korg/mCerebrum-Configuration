# EMA

## Configuration
Create EMA questions from https://surveyjs.io/Survey/Builder/

#### Supported fields

| Question Type    | Description  | Options| Example|
| --------- | ---| --- | ---------|
| text      | input text question.|<b>InputType</b>: color, date, datetime, email, month, number, password, range, tel, text, time, url, week||
| Radio Group| multiple choice question|
| Check Box |       |
| Image Picker |       |
| Dropdown |       |
| Rating |      |
| Matrix Single Choice | |
| Date Range||
| Number Chooser|
| Seekbar|
| star_rating|
| image capture|
| video capture|

| base fields    | Description  | Example|
| ------------- | ---| ----- |
|`name`|question id|`"name": "stress_question"`|
|`title`|Title of the question |`"title": "Are you stressed?"`|
|`titleLocation`|default, top, bottom, left|`"titleLocation": "top"`|
|`defaultValue`| default answer of th question | `"defaultValue": "abc"`|
|`enableIf`|  | `"enableIf": "{question13} notempty and {question13} >= 5`"
|`isRequired`| user needs to answer| `"isRequired": true`|
|`requiredErrorText`| show message if not answered| `"requiredErrorText":"Invalid input"`|
|`useDisplayValuesInTitle`|
|`visible`|
|`visibleIf`| |"visibleIf": "{question13} notempty and {question13} >= 5"|
|`hasComment`<br>`commentText`|

| Checkbox    | Description  | Example|
| ------------- | ---| ----- |
|`choices:[]`<br>`value`<br>`text`| List of choices| `"choices": [{"value": "stressed, "text": "Stressed"}]`|
|`hasNone`<br>`noneText`| Is none option  |
|`hasSelectAll`<br>`selectAllText`|||
|`hasOther`<br>`otherText` <br>`otherErrorText`|conditional expression ||
|`colCount`|


| RadioGroup    | Description  | Example|
| ------------- | ---| ----- |
|`choices:[]`<br>`value`<br>`text`| List of choices| `"choices": [{"value": "stressed, "text": "Stressed"}]`|
|`hasOther`<br>`otherText` <br>`otherErrorText`|conditional expression ||
|`colCount`|

| Dropdown    | Description  | Example|
| ------------- | ---| ----- |
|`choices:[]`<br>`value`<br>`text`| List of choices| `"choices": [{"value": "stressed, "text": "Stressed"}]`|
|`hasOther`<br>`otherText` <br>`otherErrorText`|conditional expression ||
|`colCount`|
|`optionsCaption`|

| Rating    | Description  | Example|
| ------------- | ---| ----- |
|`rateMin`<br>`rateMax`<br>`rteValues`<br>`rateStep`| List of choices| `"choices": [{"value": "stressed, "text": "Stressed"}]`|
|`hasOther`<br>`otherText` <br>`otherErrorText`|conditional expression ||
|`maxRateDescription`<br>`minRateDescription`|


#### Conditions

| DataSource Type        | DataSource Id           | Description  | Frequency |
| ------------- |:-------------:| -----:| ------: |
| APP_USE      |  | User interaction with the app | ON_CHANGE|
| SYSTEM_LOG      |       |   connectivity,  | ON_CHANGE |

## Configure AutoSense sensors:

#### Sample:
`json
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
`
#### Configuration fields
| Field        | Description           | Default Value  |
| ------------- |:-------------| -----:|
| number_of_device_required      |  | null |
| run_as_foreground_service      | (ANDROID ONLY) Set the background service as foreground      |   "false" |
| log_app_usage | Log user interaction to the app   |    $1 |
|log_system_status| | |
|permission_to_edit_configuration| | |
|devices| | |
