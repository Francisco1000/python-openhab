python library for accessing the openHAB REST API
============
  This library allows for easily accessing the openHAB REST API.
  A number of features are implemented but not all, this is work in progress.

Requirements
------------
  - python 2.7.x
  - python-dateutil
  - python-requests

Example
------------
  ```python
  import openhab
  
  base_url = 'http://localhost:8080/rest'
  
  # fetch all items
  items = openhab.fetch_all_items(base_url)
  
  sunset = items.get('Sunset')
  print sunset.state
  ```