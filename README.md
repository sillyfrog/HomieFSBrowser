# HomieFSBrowser
A quick hack to provide the File System Browser example to run along side a Homie implementation

See https://github.com/sillyfrog/homie_water_level for an example of it in use. 

By default provides a web server on port 88, for example at  ```http://homie.local:88/edit``` to browse and upload the files on the local filesystem (SPIFFS), this is mostly the FSBrowser.ino example provided with the ESP8266 libraries.

Basically all you need to do is:

```
#include <HomieFSBrowser.h>
```

Then at the end of your ```setup()``` function:

```
fsSetup();
```

And finally at the end of your ```loop()``` function:

```
fsLoop();
```
