My Home Assistant config files including products of:

* [AVM](https://avm.de)
* [Ecovacs](https://ecovacs.com)
* [Eurotronic](https://eurotronic.org)
* [Rademacher](https://rademacher.de/)
* [Roon](https://roonlabs.com/)
* [Sonos](https://sonos.com)

## Features

* A [script](https://github.com/florib779/homeassistant-config/blob/master/packages/gitpush/gitpush.sh) which automatically pushes to GitHub
* A [modified Roon Web Display](https://florib779.github.io/Roon/articles/roon-web-display.html)
* A [ROCK dashboard](https://florib779.github.io/Roon/articles/home-assistant-roon-rock-view.html)
* Sonos
  - [x] Night mode (does not work when playing music via roon) via [Sonos integration](https://www.home-assistant.io/integrations/sonos)
  - [x] Speech enhancement (does not work when playing music via roon) via [Sonos integration](https://www.home-assistant.io/integrations/sonos)
  - [x] Speaker group management via [Mini Media Player](https://github.com/kalkih/mini-media-player)
  - [x] Bass/Treble via [node-sonos-http-api](https://github.com/jishi/node-sonos-http-api)
  - [ ] Loudness (seems to be not possible yet)
  - [ ] Balance (seems to be not possible yet)
  - [x] Control subwoofer via [node-sonos-http-api](https://github.com/jishi/node-sonos-http-api)
    - [x] On/Off
    - [x] Volume level
    - [x] Crossover frequency
    - [x] Polarity
  - [x] Control status lights via [Sonos integration](https://www.home-assistant.io/integrations/sonos)
  - [x] Control buttons via [Sonos integration](https://www.home-assistant.io/integrations/sonos)
* Roon
  - [x] Control/Show info
    - [x] [RoonLabs music player integration](https://www.home-assistant.io/integrations/roon/)
      - [ ] Transfer zones
    - [ ] Remote control with [roon-cec-controller-extension](https://github.com/benjaminbellamy/roon-cec-controller-extension)
      - [x] Start/pause
      - [ ] ~Forward~ (my remote control does not send a cec command for this)
      - [ ] ~Backward~ (my remote control does not send a cec command for this)
      - [ ] Fast forward (has to be modified)
      - [x] Rewind
      - [ ] ~Volume~ (my remote control does not send a command for this)
* TV
  - [x] Turn TV on via [Wake on LAN integration](https://www.home-assistant.io/integrations/wake_on_lan/)
  - [x] Turn TV off via [Android TV integration](https://www.home-assistant.io/integrations/androidtv/)
  - [x] Control TV
    - [Android TV integration](https://www.home-assistant.io/integrations/androidtv/)
  - [x] [Notifications for Android TV / FireTV ](https://www.home-assistant.io/integrations/nfandroidtv/)
* AVM FRITZ!Box
  - [x] Sensor for internet connectivity (with external IP and uptime attributes) via [AVM FRITZ!Box Tools integration](https://www.home-assistant.io/integrations/fritz/)
  - [x] Turn wifi and guest wifi on/off [FRITZ!Box Tools](https://github.com/mammuth/ha-fritzbox-tools)
* AVM FRITZ!DECT devices
  * Control
    - [x] Eurotronic Comet DECT (radiator control - similar to FRITZ!DECT 300)
    - [x] AVM FRITZ!DECT 200 (smart plug)
    - [x] AVM FRITZ!DECT 210 (smart plug)
    - [x] AVM FRITZ!DECT 300 (radiator control)
    - [ ] AVM FRITZ!DECT 440 (push button switch)
    - [ ] AVM FRITZ!DECT 500 (LED light) - actually not implemented in Home Assistant
    - [ ] Rademacher RolloTron DECT 1213 (shutter) - controlling is actually not implemented in Home Assistant
      - [ ] Close shutter when TV is turned on
      - [ ] Go to favorite position at a given time
  * Show info
    - [x] Eurotronic Comet DECT (radiator control)
    - [x] Deutsche Telekom/Eurotronic 40318684 (door/window contact)
    - [x] AVM FRITZ!DECT 200 (smart plug)
    - [x] AVM FRITZ!DECT 210 (smart plug)
    - [x] AVM FRITZ!DECT 300 (radiator control)
    - [x] AVM FRITZ!DECT 440 (push button switch)
      - [x] Temperature
      - [ ] Humidity (actually not implemented in Home Assistant)
    - [x] Rademacher RolloTron DECT 1213 (shutter)
      - Indicates whether it is open or closed
* Ecovacs Deebot ([lovelace-xiaomi-vacuum-card](https://github.com/benct/lovelace-xiaomi-vacuum-card))
  - [x] Control
  - [x] Show info
- [x] Cooking Timer

## Links

* https://github.com/christian-ek/home-assistant-config - a lot of inspiration, especially for Sonos.