# Interface Digital Twins




### Location attributes
The following types are supported and returned by the geocoder in both the address type and address component type arrays:
- `street_address` indicates a precise street address
- `street_number` indicates the precise street number
- `country` indicates the national political entity, and is typically the highest order type returned by the Geocoder
- `administrative_area_level_1` indicates a first-order civil entity below the country level. Within the United States, these administrative levels are states. Not all nations exhibit these administrative levels. In most cases, administrative_area_level_1 short names will closely match ISO 3166-2 subdivisions and other widely circulated lists; however this is not guaranteed as our geocoding results are based on a variety of signals and location data.
- `administrative_area_level_2` indicates a second-order civil entity below the country level. Within the United States, these administrative levels are counties. Not all nations exhibit these administrative levels.
- `administrative_area_level_3` indicates a third-order civil entity below the country level. This type indicates a minor civil division. Not all nations exhibit these administrative levels.
- `administrative_area_level_4` indicates a fourth-order civil entity below the country level. This type indicates a minor civil division. Not all nations exhibit these administrative levels.
- `administrative_area_level_5` indicates a fifth-order civil entity below the country level. This type indicates a minor civil division. Not all nations exhibit these administrative levels.
- `locality` indicates an incorporated city or town political entity.
- `sublocality` indicates a first-order civil entity below a locality. For some locations may receive one of the additional types: sublocality_level_1 to sublocality_level_5. Each sublocality level is a civil entity. Larger numbers indicate a smaller geographic area.
- `sublocality_level_1` indicates a first-order civil entity below a locality. For some locations may receive one of the additional types: sublocality_level_1 to sublocality_level_5. Each sublocality level is a civil entity. Larger numbers indicate a smaller geographic area.
- `sublocality_level_2` indicates a first-order civil entity below a locality. For some locations may receive one of the additional types: sublocality_level_1 to sublocality_level_5. Each sublocality level is a civil entity. Larger numbers indicate a smaller geographic area.
- `sublocality_level_3` indicates a first-order civil entity below a locality. For some locations may receive one of the additional types: sublocality_level_1 to sublocality_level_5. Each sublocality level is a civil entity. Larger numbers indicate a smaller geographic area.
- `sublocality_level_4` indicates a first-order civil entity below a locality. For some locations may receive one of the additional types: sublocality_level_1 to sublocality_level_5. Each sublocality level is a civil entity. Larger numbers indicate a smaller geographic area.
- `sublocality_level_5` indicates a first-order civil entity below a locality. For some locations may receive one of the additional types: sublocality_level_1 to sublocality_level_5. Each sublocality level is a civil entity. Larger numbers indicate a smaller geographic area.
- neighborhood indicates a named neighborhood
- premise indicates a named location, usually a building or collection of buildings with a common name
- subpremise indicates a first-order entity below a named location, usually a singular building within a collection of buildings with a common name
- `plus_code` indicates an encoded location reference, derived from latitude and longitude. Plus codes can be used as a replacement for street addresses in places where they do not exist (where buildings are not numbered or streets are not named). See https://plus.codes for details.
- `postal_code` indicates a postal code as used to address postal mail within the country.
- `floor` indicates the floor of a building address.
- `room` indicates the room of a building address.
- bus_station, train_station and transit_station indicate the location of a bus, train or public transit stop.


```json
{
  "id":"",
  "visibility":"",
  "version":"",
  "status":"",
  "product":{
    "id":"",
    "make":"",
    "model":"",
    "year":"",
    "version":"",
    "code":"",
    "size":{
      "unit":"",
      "width":"",
      "height":"",
      "depth":""
    },
    "weight":{
      "unit":"",
      "value":""
    }
  },
  "location":{
    "gps":{
      "lat":"",
      "lon":"",
      "el":""
    },
    "address":{
		"street_address":"",
		"country":"",
		"administrative_area_level_1":"",
		"administrative_area_level_2":"",
		"administrative_area_level_3":"",
		"administrative_area_level_4":"",
		"administrative_area_level_5":"",
		"locality":"",
		"sublocality":"",
		"sublocality_level_1":"",
		"sublocality_level_2":"",
		"sublocality_level_3":"",
		"sublocality_level_4":"",
		"sublocality_level_5":"",
		"postal_code":""
    },
    "complex":{
      "premise":"",
      "subpremise":"",
      "floor":"",
      "room":"",
      "spot":""
    }
  },
  "details":{
    "author":{
      "id":"",
      "firstname":""
    }
  },
  "structure":{
    "front":{
      "label":"x",
      "description":"x",
      "width":
      "height":
      "items":
        "rows":[
          {
            "name":"",
            "label":"products",
            "description":"products",
            "height:"50%",
            "items":[
              {
                "label":"i18n()",
                "description":"i18n(key)",
                "type":"button|dial|touch|display|touchdisplay|knob|slider",
                "":"flat|emboss|inset|touch"
                "color":"#FF3300"
                "shape":"rectangular|square|oval|diamond|",
                "width":
                "height":
                "depth":
                "options":[
                  {
                    "name":"",
                    "description":""
                  }
                ]
              }
            ]
          }
        ],
        "columns":[
          {
            "
          }
        ],
        "grid":{
          "label":"x",
          "description":"x",
          "type":"x",
          
        }
    },
    "back":{
      
    },
    "left":{
      
    },
    "right":{
      
    },
    "top":{
      
    },
    "bottom":{
      
    }
  },
  "applications":{
    "pepsi":{}
  },
  "i18n":{
    "options":
    {
      "fallback":"en",
      "generate":true
    },
    "languages":{
      "en":{
        "options":{
          "fallback":"en",
          "generate":false
        },
        "keys":{
          "k":"v"
        }
      }
    }
  }
}
```