My Home Assistant config files including products of:

* AVM
* Ecovacs
* Roon
* Sonos

## Features

Includes:
* A script (`ha_gitpush.sh`) which automatically pushes to GitHub ([see](https://peyanski.com/automatic-home-assistant-backup-to-github/))
* A [modified Roon Web Display](https://florib779.github.io/Roon/articles/roon-web-display.html)
* A [ROCK dashboard](https://florib779.github.io/Roon/articles/home-assistant-roon-rock-view.html)
* Sonos
  - [x] Night mode (does not work when playing music via roon)
  - [x] Speech enhancement (does not work when playing music via roon)
  - [x] Speaker group management - [Mini Media Player](https://github.com/kalkih/mini-media-player) (Customizable media player card for Home Assistant Lovelace UI)
  - [ ] Bass/Treble (looking for a nice solution like [lovelace-slider-entity-row](https://github.com/thomasloven/lovelace-slider-entity-row))
  - [ ] Loudness (seems to be not possible yet)
  - [ ] Control subwoofer [node-sonos-http-api](https://github.com/jishi/node-sonos-http-api)
    - [x] On/Off
    - [ ] Volume level (looking for a nice solution like [lovelace-slider-entity-row](https://github.com/thomasloven/lovelace-slider-entity-row))
    - [ ] Crossover frequency (looking for a nice solution like [lovelace-slider-entity-row](https://github.com/thomasloven/lovelace-slider-entity-row))
    - [x] Polarity
      - ToDo: only show when Sub is on
* Roon
  - [x] Control/Show info
    - [x] [RoonLabs music player](https://www.home-assistant.io/integrations/roon/)
      - [ ] Transfer zones
    - [x] [Mini Media Player](https://github.com/kalkih/mini-media-player) (Customizable media player card for Home Assistant Lovelace UI)
    - [ ] Remote control with [roon-cec-controller-extension](https://github.com/benjaminbellamy/roon-cec-controller-extension)
      - [x] Start/pause
      - [ ] ~Forward~ (my remote control does not send a cec command for this)
      - [ ] ~Backward~ (my remote control does not send a cec command for this)
      - [ ] Fast forward (has to be modified)
      - [x] Rewind
      - [ ] ~Volume~ (my remote control does not send a command for this)
* TV
  - [x] Turn TV on [Wake on LAN](https://www.home-assistant.io/integrations/wake_on_lan/)
  - [x] Turn TV off [Android TV](https://www.home-assistant.io/integrations/androidtv/)
  - [ ] Control TV
    - [Android TV](https://www.home-assistant.io/integrations/androidtv/)
  - [ ] [Notifications for Android TV / FireTV ](https://www.home-assistant.io/integrations/androidtv/)
* AVM FRITZ!Box
  - [x] Sensor for internet connectivity (with external IP and uptime attributes) [AVM FRITZ!Box Tools](https://www.home-assistant.io/integrations/fritz/)
  - [x] Turn on/off wifi and guest wifi [FRITZ!Box Tools](https://github.com/mammuth/ha-fritzbox-tools)
* AVM FRITZ!DECT devices
  * Control
    - [x] Comet DECT (radiator control - similar to FRITZ!DECT 300)
    - [x] FRITZ!DECT 200 (smart plug)
    - [x] FRITZ!DECT 210 (smart plug)
    - [x] FRITZ!DECT 300 (radiator control)
    - [ ] FRITZ!DECT 440 (push button switch)
    - [ ] FRITZ!DECT 500 (LED light) (actually not implemented in Home Assistant)
    - [ ] Rademacher RolloTron DECT 1213 (shutter)
      - Actually not implemented in Home Assistant
      - [ ] Close shutter when TV is turned on.
      - [ ] Go to favorite position at a given time
  * Show info
    - [x] Comet DECT (radiator control)
    - [x] Deutsche Telekom/Eurotronic 40318684 (door/window contact)
    - [x] FRITZ!DECT 200 (smart plug)
    - [x] FRITZ!DECT 210 (smart plug)
    - [x] FRITZ!DECT 300 (radiator control)
    - [x] FRITZ!DECT 440 (push button switch with temperature sensor)
      - [x] Temperature
      - [ ] Humidity (actually not implemented in Home Assistant)
    - [x] Rademacher RolloTron DECT 1213 (shutter)
* Ecovacs Deebot [lovelace-xiaomi-vacuum-card](https://github.com/benct/lovelace-xiaomi-vacuum-card)
  - [x] Control
  - [x] Show info
- [x] Cooking Timer
- [ ] Alarm Clock
  * [Hass-Custom-Alarm](https://github.com/akasma74/hass-custom-alarm)
- [ ] Report the amount of unread emails - [IMAP](https://www.home-assistant.io/integrations/imap/)