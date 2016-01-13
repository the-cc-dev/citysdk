# Global





* * *

## Class: CkanModule
Instantiates an instance of the CitySDK CKAN object.

### CkanModule.enable(apiKey) 

Enable function. Stores the API key for this module and sets it as enabled.  It will also compare the CitySDK core's version number to the minimum number required as specified for this module.

**Parameters**

**apiKey**: `string`, The census API key.

**Returns**: `boolean`, True if enabled, false is not enabled.

### CkanModule.search(request, callback) 

Sends a SQL query to a CKAN server.

**Parameters**

**request**: `object`, JSON Object

**callback**: `function`, Sends a SQL query to a CKAN server.

**Returns**: `object`, JSON Object



* * *









