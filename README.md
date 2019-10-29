[![License](https://img.shields.io/github/license/abdian/ha-datetimepicker.svg?style=flat)](LICENSE)

This is a fork of hossein-alipour's [ha-datetimepicker](https://github.com/hossein-alipour/ha-datetimepicker) which adds 24 Hours format.

# HA-DateTimePicker (with 24 hours format)
A date and time picker with Solar (Persian), Lunar (Arabic) and Gregorian calendars.

# Installation
Download the files and include them in your project.

JS Files:
```html
<script type="text/javascript" src="ha-solardate.min.js"></script>
<script type="text/javascript" src="ha-lunardate.min.js"></script> <!-- If you don't need the lunar calendar features, just ignore this line -->
<script type="text/javascript" src="ha-datetimepicker.min.js"></script>
```
*Note: Be sure to include the ha-solardate.js and ha-lunardate.js file before ha-datetimepicker.js*

CSS File:
```html
<link rel="stylesheet" type="text/css" href="ha-datetimepicker.min.css" />
```


# How to use
### 1. Add `data-ha-datetimepicker` attribute to your DOMElement.
```html
<input type="text" id="datetime" data-ha-dp-is24="true" data-ha-datetimepicker="#datetime" />
```

### 2. Show using Javascript.

  ```javascript
  var dp = new HaDateTimePicker("#datetime");
  dp.show();
  ```
  
# Features
You can initiate your `HA-DateTimePicker` with this set of options:

*Note: you can use this features with javascript object or HTML Attribute*

Javascript option | HTML attribute | Type | description
------------ | ------------- | ------------- | -------------
is24 | data-ha-dp-is24 | Boolean | Use 24 hours mode
date | data-ha-dp-date | Date | Initial month and year sheet
selectedDate | data-ha-dp-selecteddate | Date | Selected Date
minYear | data-ha-dp-minyear | Number | The first year in the year dropdown list
maxYear | data-ha-dp-maxyear | Number | The last year in the year dropdown list
isSolar | data-ha-dp-issolar | Boolean | Turns into Solar(Persian) Calendar
isLunar | data-ha-dp-islunar | Boolean | Turns into Lunar(Arabic) Calendar
resultInSolar | data-ha-dp-resultinsolar | Boolean | Returns the result in Solar(Persian) date mode
resultInLunar | data-ha-dp-resultinlunar | Boolean | Returns the result in Lunar(Arabic) date mode
forceSetTime | data-ha-dp-forcesettime | Boolean | Forces the user to set the time
disableTime | data-ha-dp-disabletime | Boolean | Disables the time feature
pagingDuration | data-ha-dp-pagingduration | Number | The duration time of changing month (In Miliseconds)
minAllowedDate | data-ha-dp-minalloweddate | Date | The minimum date that the user can select
maxAllowedDate | data-ha-dp-maxalloweddate | Date | The maximum date that the user can select
resultFormat | data-ha-dp-resultformat | String | The string format of date and time result. use {year} for year, {month} for month, {day} for day, {hour} for hour, {minute} for minute, {ampm} for AM or Pm and if you want to display some text only when time is available put it between {t? and }. ex. {month}/{day}/{year} {t?{hour}:{minute} {ampm}}
disabledWeekDays | data-ha-dp-disabledweekdays | Array or String(separated by comma) | Use the number of week days to disable them.  1 for Sunday(یکشنبه or الأحد) and 7 for Saturday(شنبه or السبت)


# Changelog
v1.5
 - Added 24 Hours format

v1.4 and before
- Please checkout [original project](https://github.com/hossein-alipour/ha-datetimepicker)'s changelog.

## Acknowledgments
Special thanks to [hossein-alipour](https://github.com/hossein-alipour) for the original [project](https://github.com/hossein-alipour/ha-datetimepicker).

## License
- This project is licensed under the [MIT License](LICENSE).
- The [original project](https://github.com/hossein-alipour/ha-datetimepicker) is licensed under the [MIT License](https://opensource.org/licenses/MIT).
