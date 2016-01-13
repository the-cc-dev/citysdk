# Global





* * *

## Class: FarmersMarketModule
Instantiates an instance of the CitySDK Farmer's Market object.

### FarmersMarketModule.enable(apiKey) 

Enable function. Stores the API key for this module and sets it as enabled.  It will also compare the CitySDK core's version number to the minimum number required as specified for this module.

**Parameters**

**apiKey**: `string`, The census API key.

**Returns**: `boolean`, True if enabled, false is not enabled.

### FarmersMarketModule.search(request, callback) 

Searches near a specified lat/lng or zipcode

**Parameters**

**request**: `object`, JSON request

**callback**: `function`, Searches near a specified lat/lng or zipcode

**Returns**: `object`, <pre><code>{

### FarmersMarketModule.detail(request, callback) 

Requests details about the farmer's market with specified id

**Parameters**

**request**: `object`, JSON request

**callback**: `function`, Requests details about the farmer's market with specified id

**Returns**: `object`, <pre><code>{



* * *









