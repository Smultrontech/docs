# BrewPiLess

Check the [BrewPiLess documentation](https://github.com/vitotai/BrewPiLess/wiki/Logging-to-Brewfather) for setup instructions. You will find the ID in the URL in Brewfather settings.

### Option 1

Go into the settings page in [Brewfather APP](https://web.brewfather.app/), enable [Brewpiless](https://github.com/vitotai/BrewPiLess). Copy the ID from the **URL** to copy into the Brewpiless remote logging configuration page. Select Brewfather as logging type, and paste the id.

After the Brewpiless has done its first logging to Brewfather, it will appear in the device list located in your Batch &gt; Fermentation &gt; Readings &gt; **Devices**. Click on the Devices button and attatch your Brewpiless to the batch. The next time your Brewpiless logs, it will show up in your batch!

**Never log more than once every 15 minutes**, request logged more often than that will be ignored.

### Option 2

Go into the settings page in [Brewfather APP](https://web.brewfather.app/), enable [Brewpiless](https://github.com/vitotai/BrewPiLess). You will then get a **URL**, **Data Type** and **Format** that you need to copy into the Brewpiless remote logging configuration page use remote logging type.

**Set log time period to 900 seconds**. Your Brewpiless should then log every 15 minutes.

After the Brewpiless has done its first logging to Brewfather, it will appear in the device list located in your Batch &gt; Fermentation &gt; Readings &gt; **Devices**. Click on the Devices button and attatch your Brewpiless to the batch. The next time your Brewpiless logs, it will show up in your batch!

**Never log more than once every 15 minutes**, request logged more often than that will be ignored.

#### Logging format

{"id":"FERMENTER1","tempUnit":"C","beerTemp":%b,"beerSet":%B,"fridgeTemp":%f,"fridgeSet":%F,"roomTemp":%r,"gravity":%g,"tiltValue":%t,"auxTemp":%a,"extVolt":%v,"timestamp":%u}

**tempUnit** can be C for celcius, F for fahrenheit or K for kelvin.

### Multiple devices

Having multiple BPL logging to Brewfather is simple, just set them all up logging to the same URL, but make sure they have unique an unique id in the configuration. Example above shows "FERMENTER1" as id. Newer BPL

