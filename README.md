# Prayer Times Web API

C# .NET WEBAPI to get prayer times in one day or annual (Base on university of Tehran calculations)

## Rest API with JSON standard output

## Websites for API:
* https://syber.ir (Primary)
* https://mamijob.ir (Alternative)

# Documentation & Usage

### Quick Start sample
https://mamijob.ir/api/oghat/53.55/9.9/999/0/
* latitude = 53.55
* longitude = 9.9

Results:
```javascript
{
  imsakString: "02 : 24",
  modifiedFajrString: "02 : 54",
  riseString: "05 : 55",
  noonString: "14 : 24",
  asrString: "18 : 50",
  setString: "22 : 53",
  maghribString: "23 : 29",
  modifiedIshaString: "",
  midnightString: "00 : 54"
}
```
# 1. One day result
---
## 1.1. country NOT in EU DTS timezone (NORMAL HOUR) // 999 means today

### 1.1.1 Calculate today
*  https://mamijob.ir/api/oghat/lat/lng/999/newYear/1/1/24/1/1/24/
*  https://syber.ir/api/oghat/lat/lng/999/newYear/1/1/24/1/1/24/


### 1.1.2 Calculate specific day of year
* https://mamijob.ir/api/oghat/lat/lng/dayOfYear/newYear/1/1/24/1/1/24/
* https://syber.ir/api/oghat/lat/lng/dayOfYear/newYear/1/1/24/1/1/24/


## 1.2. country in EU DTS timezone 

 ### 1.2.1. Calculate today (annual prayer times) 
 * https://mamijob.ir/api/oghat/lat/lng/999/0/
 * https://syber.ir/api/oghat/lat/lng/999/0/

### 1.2.2. Calculate specific day of year
* https://mamijob.ir/api/oghat/lat/lng/dayOfYear/newYear/
* https://syber.ir/api/oghat/lat/lng/dayOfYear/newYear/

lat = latitude of the point

lng = longitude of the point

dayOfYear = number of day in year


 # 2.Annual prayer times (365 Days)
 ---
 ## 2.1 Country NOT EU DTS (NORMAL HOUR)
 * https://mamijob.ir/api/alloghat/lat/lng/year/0/1/1/24/1/1/24/
 * https://syber.ir/api/alloghat/lat/lng/year/0/1/1/24/1/1/24/
 
 ## 2.2 Country is EU DTS 
 * https://mamijob.ir/api/alloghat/lat/lng/year/
 * https://syber.ir/api/alloghat/lat/lng/year/


lat = latitude

lng = longitude

year = the year that you want to calculate
