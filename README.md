# Mac OS Wifi Scanner

There is no `iwlist` on Mac OS, that is why I've created my own script to get all SSID around me via cli ;) 


## Prerequisites:

Before running anything, check out the `requirements.txt` and make sure you have everything neccessary to run this script installed. To install all needed requirements:

```bash
pip install -r requirements.txt
```

Then run a script:

```bash

python3 wifi-scan.py

```


## Example:

How to use it:

```bash
python3 wifi-scan.py

{'SOME WIFI': {'RSSI': -45, 'channel': balabala, 'noise': -92},
 'ANOTHER_WIFI': {'RSSI': -50, 'channel': qwqwqwq, 'noise': -92}}

```

Wifi-scan.py support `filter` argument, which can be used to find any particular SSID.

```bash
python3 wifi-scan.py -f SOME_WIFI

{'SOME WIFI': {'RSSI': -45, 'channel': balabala, 'noise': -92}

```
