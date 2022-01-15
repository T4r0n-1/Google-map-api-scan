# Google-map-api-scan

# Google Maps API Scanner
Used for determining whether a leaked/found Google Maps API Key is vulnerable to unauthorized access by other applications or not.  

***Usage:***
- Download `maps_api_scanner.py` file and run as: `python maps_api_scanner.py` & paste API key wanted to test when asked. 
- Script will return `API key is vulnerable for XXX API!` message and the PoC link/code if determines any unauthorized access within this API key within any API's.
- Now it supports also api key as argument such as `python maps_api_scanner.py --api-key API_KEY`. 
- If you want to use `python3`, download `maps_api_scanner_python3.py` file and run as: `python3 maps_api_scanner_python3.py`.

***Checked APIs:***
- Staticmap API
- Streetview API
- Embed (Basic-Free) API
- Embed (Advanced-Paid) API
- Directions API
- Geocode API
- Distance Matrix API
- Find Place From Text API
- Autocomplete API
- Elevation API
- Timezone API
- Roads API
- Geolocation API
- Route to Traveled API
- Speed Limit-Roads API
- Place Details API
- Nearby Search-Places API
- Text Search-Places API
- Places Photo API
- Playable Locations API
- FCM API
- Custom Search API

***Semi-Auto Checked APIs:***
- JavaScript API

***Notes:***
- Because JavaScript API needs manual confirmation from a web browser directly, only file is created via the script for manual checks/confirmation.
- For Staticmap, Streetview and Embed API's, if used from another domain instead of just testing from browser; whether referer checks are enabled or not on the server-side for the key, script still could return it as vulnerable due to a server-side vulnerability. If you cannot reproduce the vulnerability via browser while the script says so, please read the ***Blog Post #2*** for more information & a better understanding about what is going on. 
- If you find any Google Maps API's which are not mentioned in this document/script, create an issue with details so I can also add them.
- Special thanks to [Yatin](https://twitter.com/ysirpaul) for his contributions on both discovery of additional API's & cost information!
