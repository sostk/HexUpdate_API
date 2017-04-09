# HexUpdate_API

To help you add ota to your device, follow the advice below.

First you should put the following line in your device's system.prop, or any place that adds the same to build.prop.

      #OTA Hexagon
      hex.updater.uri=https://raw.githubusercontent.com/HexagonRom/HexUpdate_API/hex-7.1/codename-your-device.json
      
You should now create a new "json" file from your device for this repository.

      https://github.com/HexagonRom/HexUpdate_API
      
Create file name codename-your-device.json and add this:

      {
        "response": [
          {
            "datetime": ???, 
            "filename": "???", 
            "id": "???", 
            "romtype": "official", 
            "url": "???",
            "version": "2.3"
          }
        ]
      }
      
 # See for name:
 After you finish compiling a build, before uploading, you need to type this into your terminal:
       date +%s
 
 It will generate a number, it is used in your "json" file in the local datetime.
 
 # See
 datetime = number generate
 filename = Name file zip rom
 id = MD5sum
 url = Direct link for download
 
 Create this in pull request if you have no rights in the organization, and soon we will merge it.
