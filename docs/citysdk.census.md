# Global





* * *

### enable(apiKey) 

Enable function. Stores the API key for this module and sets it as enabled.  It will also compare the CitySDK core's version number to the minimum number required as specified for this module.

**Parameters**

**apiKey**: `string`, The census API key.

**Returns**: `boolean`, True if enabled, false is not enabled.


### parseToVariable(aliasOrVariable) 

Checks to see if a string is in the aliases dictionary and returns the appropriate variable if so.

**Parameters**

**aliasOrVariable**: `string`, A string to parse into a variable string.

**Returns**: `string`, Variable string


### parseToValidVariable(aliasOrVariable, api, year) 

Checks to see if a string is in the aliases dictionary and returns the appropriate VALID variable if so.

**Parameters**

**aliasOrVariable**: `string`, A string to parse into a variable string.

**api**: `string`, The api key being called (acs5, sf1, etc)

**year**: `string`, The year of the desired dataset

**Returns**: `string`, Variable string


### isNormalizable(alias) 

Returns TRUE if the alias is normalizable (as marked in the alias dictionary), otherwise, false.

**Parameters**

**alias**: `string`, Returns TRUE if the alias is normalizable (as marked in the alias dictionary), otherwise, false.

**Returns**: `boolean`


### parseRequestStateCode(request) 

Parses the state code in a request object, converting two letter state codes to lat/lng

**Parameters**

**request**: `object`, Object representing an api request



### parseRequestLatLng(request) 

Checks the request object for lat/lng latitude/longitude and x/y fields and moves them to the appropriate locations

**Parameters**

**request**: `object`, Object representing an api request



### ESRItoGEO(esriJSON) 

Converts ESRI JSON to GeoJSON

**Parameters**

**esriJSON**: `string`, Converts ESRI JSON to GeoJSON

**Returns**: `Object`


### GEOtoESRI(geoJSON) 

Converts geoJSON to ESRI Json

**Parameters**

**geoJSON**: , Converts geoJSON to ESRI Json

**Returns**: `*`


### getVariableDictionary(api, year, callback) 

Downloads an ACS API's entire dictionary of variables from the Census

**Parameters**

**api**: `string`, Downloads an ACS API's entire dictionary of variables from the Census

**year**: `string`, Downloads an ACS API's entire dictionary of variables from the Census

**callback**: `function`, Downloads an ACS API's entire dictionary of variables from the Census



### latLngToFIPS(lat, lng, callback) 

Converts co-ordinates to Census FIPS via the Geocoder API

**Parameters**

**lat**: `float`, Latitude

**lng**: `float`, Longitude

**callback**: `function`, Callback function



### addressToFIPS(street, city, state, callback) 

Converts a street address to Census FIPS via the Geocoder API

**Parameters**

**street**: `string`, Street Address

**city**: `string`, City

**state**: `string`, State (2-Letter USPS Code)

**callback**: `function`, Callback function



### ZIPtoLatLng(zip, callback) 

Converts a ZIP code to Lat/Lng and calls the callback on it.

**Parameters**

**zip**: `Number`, 5 digit Zip code

**callback**: `function`, Converts a ZIP code to Lat/Lng and calls the callback on it.



### summaryRequest(request, callback) 

Makes a request to the ACS5 Summary API. Should be used via APIRequest and not on its own, typically

**Parameters**

**request**: `object`, JSON request (see APIRequest)

**callback**: `function`, Makes a request to the ACS5 Summary API. Should be used via APIRequest and not on its own, typically



### tigerwebRequest(request, callback) 

Makes a call to the Census TigerWeb API for Geometry.

**Parameters**

**request**: `object`, Makes a call to the Census TigerWeb API for Geometry.

**callback**: `function`, Makes a call to the Census TigerWeb API for Geometry.



### APIRequest(request, callback) 

Processes a data request by looking at a JSON request

**Parameters**

**request**: `object`, The JSON object of the request

**callback**: `function`, A callback, which accepts a response parameter



### validateRequestGeographyVariables(requestIn, callback) 

Checks the geo-related parts of the request against the geography definition of the API being requested

**Parameters**

**requestIn**: `object`, Checks the geo-related parts of the request against the geography definition of the API being requested

**callback**: `function`, Checks the geo-related parts of the request against the geography definition of the API being requested



### validateRequestGeographyVariablesProcess(requestIn, callback) 

Compares the geoDefinition against the request.  Returns false if location variables required by the api are missing.

**Parameters**

**requestIn**: `object`, Compares the geoDefinition against the request.  Returns false if location variables required by the api are missing.

**callback**: `function`, Compares the geoDefinition against the request.  Returns false if location variables required by the api are missing.



### GEORequest(request, callback) 

Retrieves data and geographic shapes encoded as geoJSON.

**Parameters**

**request**: `object`, The JSON request

**callback**: `function`, The callback to take the response, which is geoJSON




* * *









