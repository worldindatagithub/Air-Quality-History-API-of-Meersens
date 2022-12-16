# Meersens Air Quality History API and how to work with it #
The Meersens air quality history API allows developers to retrieve hourly data on past air quality at a specific location. This tool is useful for those looking to access historical information on air quality in order to analyze trends or assess the impacts of certain factors. The primary purpose of the API is to provide a means for fetching this data quickly and efficiently.


[Air Quality History API](https://www.worldindata.com/api/Meersens-air-quality-history-api)

Worldindata's API marketplace offers a variety of third party APIs, all designed with user-friendliness in mind. These APIs aim to make it easy for developers to access and utilize the data and functionality they provide, without requiring extensive knowledge or technical expertise. By offering a curated selection of APIs that are straightforward to use, Worldindata helps to streamline the process of integration and data retrieval for developers.

## Industry, Sectors, and Customers for the API ##

**Industry and Sectors**
- weather
- air quality
- environment

**Client Types**
- weather platforms
- air quality analysts
- environment and climate change platforms
- and more



## Parameters, Objects and JSON output of the API ##
The GET /environment/public/air/history endpoint allows developers to retrieve historical air quality data for a specific location.


**Filter Parameters**
- lat
- lng
- from
- to
- index_type


```
{
    "found": true,
    "values": [
        {
            "datetime": "2021-11-07T22:00:00.000Z",
            "pollutants": {    
                "no2": {
                    "found": true,
                    "name": "Nitrogen dioxide",
                    "shortcode": "NO2",
                    "unit": "µg/m³",
                    "value": 11.3,
                    "confidence": 4.5,
                    "index": {
                        "index_type": "meersens",
                        "index_name": "Meersens",
                        "qualification": "Good",
                        "icon": null,
                        "color": "#05b3a4",
                        "description": "That air quality level won’t present a risk for health for an exposure time superior to decades",
                        "value": 9.61
                    }
                },
                "co": {...},
                "o3": {...},
                "pm10": {...},
                "pm25": {...},
                "so2": {...}
            },
            "index": {
                "index_type": "meersens",
                "index_name": "Meersens",
                "qualification": "Correct",
                "icon": null,
                "color": "#44b001",
                "value": 32.62,
                "main_pollutants": [
                    "o3"
                ]
            },
            "found": true
        },
        {...}
    ]
}

```
**Objects**
- found
- values
- values.datetime
- values.index
- values.index.index_type
- values.index.index_name
- values.index.qualification
- values.index.description
- values.index.icon
- values.index.color
- values.index.value
- values.index.main_pollutants
- values.pollutants
- values.pollutants.shortcode
- values.pollutants.name
- values.pollutants.unit
- values.pollutants.found
- values.pollutants.value
- values.pollutants.confidence
- values.pollutants.index

## SDKs ##
Our software development kits (SDKs) for the Meersens historical air quality database are available in a variety of programming languages, including JAVA, Python, Ruby, and PHP. These SDKs make it easy for developers to access and work with the data provided by the API.


### Disclaimer of infringement ###
Worldindata is a platform that helps connect developers with data providers in order to make it easier to access and use data from around the world. We do not own the data provided through our API marketplace, but we are big fans of the Meersens historical air quality API and strive to make it as user-friendly as possible. It is important to note that Worldindata is not responsible for the accuracy or reliability of the data provided through our platform, and users should exercise caution when using it.

[Worldindata](https://www.worldindata.com)
