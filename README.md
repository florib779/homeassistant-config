My Home Assistant config files including products of:

* [Android](https://www.android.com/)
* [AVM](https://avm.de)
* [Ecovacs](https://ecovacs.com)
* [Eurotronic](https://eurotronic.org)
* [Ezviz](https://www.ezvizlife.com/)
* [Govee](https://govee.com)
* [Rademacher](https://rademacher.de/)
* [Roon](https://roonlabs.com/)
* [Sonos](https://sonos.com)

## Features and goals

- [x] A [script](https://github.com/florib779/homeassistant-config/blob/master/integrations/gitpush/gitpush.sh) which automatically pushes Home Assistant config files to GitHub.

* **Sonos**
  - [x] Night mode (does not work when playing music via roon) via [Sonos integration](https://www.home-assistant.io/integrations/sonos).
  - [x] Speech enhancement (does not work when playing music via roon) via [Sonos integration](https://www.home-assistant.io/integrations/sonos).
  - [x] Speaker group management via [Mini Media Player](https://github.com/kalkih/mini-media-player).
  - [x] Bass/Treble via [Sonos integration](https://www.home-assistant.io/integrations/sonos).
  - [x] Switch rear speakers
  - [ ] Loudness.
    * Seems to be not possible yet.
  - [ ] Balance.
    * Seems to be not possible yet.
  - [x] Rear speakers.
    - [x] On/Off.
    - [ ] Volume level.
      * Seems to be not possible yet.
  - [x] Control subwoofer via [node-sonos-http-api](https://github.com/jishi/node-sonos-http-api).
    - [x] On/Off.
    - [x] Volume level.
    - [x] Crossover frequency.
    - [x] Polarity.
  - [x] Control status lights via [Sonos integration](https://www.home-assistant.io/integrations/sonos).
    - [x] Turn on/off lights at a given time as night light
  - [x] Control buttons via [Sonos integration](https://www.home-assistant.io/integrations/sonos).
* **Roon**
  - [x] Control/Show info.
    - [x] [RoonLabs music player integration](https://www.home-assistant.io/integrations/roon/).
      - [ ] Transfer zones.
    - [ ] Remote control via [roon-cec-controller-extension](https://github.com/benjaminbellamy/roon-cec-controller-extension).
      - [ ] Start/pause.
        * Possible, but currently not enabled.
      - [ ] ~Forward.~
        * My remote control does not send a cec command for this.
      - [ ] ~Backward.~
        * My remote control does not send a cec command for this.
      - [ ] Fast forward.
        - [ ] Has to be modified.
      - [ ] Rewind.
        * Possible, but currently not enabled.
      - [ ] ~Volume.~
        * My remote control does not send a command for this.
* **AVM FRITZ!Box**
  - [x] Show internet connectivity (with external IP and uptime attributes) via [AVM FRITZ!Box Tools integration](https://www.home-assistant.io/integrations/fritz/).
  - [x] Turn wifi and guest wifi on/off via [AVM FRITZ!Box Tools integration](https://www.home-assistant.io/integrations/fritz/).
* **AVM FRITZ!DECT devices**
  * Control.
    - [x] AVM FRITZ!DECT 200 (smart plug).
    - [x] AVM FRITZ!DECT 210 (smart plug).
    - [x] AVM FRITZ!DECT 300/Eurotronic Comet DECT (radiator control).
    - [ ] AVM FRITZ!DECT 400 (push button switch).
      * Currently not implemented in Home Assistant.
    - [ ] AVM FRITZ!DECT 440 (push button switch).
      * Currently not implemented in Home Assistant.
    - [x] AVM FRITZ!DECT 500 (LED light).
    - [x] Rademacher RolloTron DECT 1213 (shutter).
      * Currently not implemented in Home Assistant.
      * Possible via Homebridge [info](https://community.home-assistant.io/t/support-rademacher-rollotron-1213-dect-with-avm-fritz-smarthome/319854/5)
      - [x] Close shutter when TV is turned on.
        * To avoid light glare.
      - [x] Close shutter depending on time and the phases of the sun.
  * Show info
    - [x] Show phone status with caller information
    - [x] Deutsche Telekom (Eurotronic) 40318684 (door/window contact).
    - [x] AVM FRITZ!DECT 200 (smart plug).
      - [x] Power consumption.
      - [x] Total power consumption.
    - [x] AVM FRITZ!DECT 210 (smart plug).
      - [x] Power Consumption.
      - [x] Total Power Consumption.
    - [x] AVM FRITZ!DECT 300/Eurotronic Comet DECT (radiator control).
      - [x] Battery level.
    - [x] AVM FRITZ!DECT 400 (push button switch).
      - [x] Battery Level.
    - [x] AVM FRITZ!DECT 440 (push button switch).
      - [x] Temperature.
      - [x] Battery Level.
      - [x] Humidity.
    - [x] Rademacher RolloTron DECT 1213 (shutter).
* **Android** (Mobile/TV)
  - [x] Control.
    - [x] Turn TV on via [Wake on LAN integration](https://www.home-assistant.io/integrations/wake_on_lan/).
    - [x] Turn TV off via [Android TV integration](https://www.home-assistant.io/integrations/androidtv/).
  - [x] Show info.
    - [x] Akku.
    - [x] Connectivity.
    - [x] Control, as with the remote control.
    - [x] Notifications/Messages.
    - [x] State.

## Automations
- [x] Presence detection.
  - [x] Music on/off.
  - [x] All devices on/off.
  - [x] Vacuum on/off.

## Links

* https://github.com/christian-ek/home-assistant-config - a lot of inspiration, especially for Sonos.
* https://gitlab.com/The3DmaN/ha-connect - HA Connect is a simple web app for connecting to the web interface of an Home Assistant server. It is designed for Linux mobile but may also run on other platforms.