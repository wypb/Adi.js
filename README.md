# Adi.js
Lightweight jQuery plugin for Adblock detection

### ```bower install adi.js```

### To install follow the steps (order is important):
  
  - Include ```jQuery```
  - Include ```advertisement.js``` and make sure ```jQuery.adblock = false;``` is inside the file
  - Include ```jquery.adi.js```
  - Call ```$.adi({ /* your options here */ })```


### Options
All parameters are optional.

|    Option     |       Type        |                        Description                        |
|---------------|-------------------|-----------------------------------------------------------|
| ```title```   | ```string/html``` | Modal's title                                             |
| ```content``` | ```string/html``` | Modal's description                                       |
| ```theme ```  | ```string```      | Available: ```light```, ```dark``` (default: ```light```) |


### Methods

|      Method      |                                                    Description                                                    |
|------------------|-------------------------------------------------------------------------------------------------------------------|
| ```active()```   | Callback function triggered when ```$.adblock``` is ```undefined```.<br> *Adblock is active*                      |
| ```inactive()``` | Callback function triggered when ```$.adblock``` is ```false```.<br> *Adblock is inactive*                        |
| ```onOpen()```   | Callback function triggered when modal is appended to ```document.body``` and ```display``` is set to ```block``` |
| ```onClose()```  | Callback function triggered when modal's ```display``` is set to ```none```                                       |

