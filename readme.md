# pico-wifi-setup (circuitpython)

**Status:** *incomplete*

## About
The idea is to be able to remotely configure a Raspberry Pi Pico (running circuitPython) so that it can connect to a home WiFi network.


## Method
Assuming a `setup` button is pressed on startup, then the following will happen:

1. Create a local wifi network called `Pico_WiFi` with password `xxxxxxxx` (8 x's)
1. Host a static website that will ask for WiFi **name** and **password**
1. Save those values to the `Settings.toml` file

When it's connected it should have an IP address printed to the terminal, which will most likely be

`Started development server on http://192.168.4.1:80`



## References

This is a project using circuitPython - info here: https://circuitpython.org/
1. https://docs.circuitpython.org/en/latest/shared-bindings/wifi/index.html#wifi.Radio.start_ap
1. https://docs.circuitpython.org/projects/httpserver/en/latest/examples.html
1. https://www.recantha.co.uk/blog/?p=21398