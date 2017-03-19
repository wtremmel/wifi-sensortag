# wifi-sensortag
Stuff I do with my TI Wifi Sensortag

# User defined tokens
* `__SL_P_UM0=` - send command to Sensortag. Possible values:
  * save = save config
  * disconnect
  * connect
  * load
  * reboot
  * default
* `__SL_P_UM4`
* `__SL_P_UM5`
* `__SL_P_UM6`
* `__SL_P_UI1=` - type of connection to IBM cloud
  * 0 = quickstart
  * 1 = registered
* `__SL_P_UIA=` - ???
* `__SL_P_UIB=` - Device ID? for quickstart URL
* `__SL_P_UIC=`
* `__SL_P_UID=` - registered organisation
* `__SL_P_UIE=` - device type
* `__SL_P_UIF=` - device ID
* `__SL_P_UIG=` - device token
* `__SL_P_UAN`  - device name (?)
* `__SL_P_UFS`
* `__SL_P_UCT`
* `__SL_P_UCF` - Sensor enable map, bitmapped:
  * 1 = Temperature
  * 2 = Humidity
  * 4 = Pressure
  * 8 = Gyroskope
  * 16 = Acceleration
  * 32 = Optical
  * 64 = Magnetic
* `__SL_P_ULD` - LED, bitmapped, 1=red, 2=green, 4=buzzer
* `__SL_P_UDV`
* `__SL_P_URG` - Write register. Syntax:
  * ="adr,len,data"

## Other Tokens
* `__SL_P_ACT` - timeout in seconds (65535 = stay on forever)

## From profiles_config.html
Add new profile:
* Target: `profiles_add.html`
* `__SL_P_P.A` - SSID
* `__SL_P_P.B` - Security type:
  * 0 = open
  * 1 = WEP
  * 2 = WPA1
  * 3 = WPA2
* `__SL_P_P.C` - security key
* `__SL_P_P.D` - priority

# URLs
* /sensortag.html
* /sys_up_time.txt
* /date_time_info.txt
* /param_product_version.txt
* /param_about.html
* /param_sensortag_conf.html
* /param_sensortag_reg.html - register info?
* /param_sensortag_poll.html - gives sensor data
  * Temperature
  * Humidity
  * Pressure
  * Gyroskope
  * Acceleration
  * Optical
  * Magnetic
  * Key (Keypress?)
  * Syn?
* Try: /sensortag.html

# Additional Documentation Found
* http://www.ti.com/lit/ug/swru455a/swru455a.pdf
