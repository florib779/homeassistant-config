My Home Assistant config files including products of:

* [Android](https://www.android.com/)
* [AVM](https://avm.de)
* [Ecovacs](https://ecovacs.com)
* [Eurotronic](https://eurotronic.org)
* [Rademacher](https://rademacher.de/)
* [Roon](https://roonlabs.com/)
* [Sonos](https://sonos.com)

## Features and goals

- [x] A [script](https://github.com/florib779/homeassistant-config/blob/master/packages/gitpush/gitpush.sh) which automatically pushes to GitHub.
- [x] A [modified Roon Web Display](https://florib779.github.io/Roon/articles/roon-web-display.html).
- [x] A [Roon ROCK dashboard](https://florib779.github.io/Roon/articles/home-assistant-roon-rock-view.html).

* **Sonos**
  - [x] Night mode (does not work when playing music via roon) via [Sonos integration](https://www.home-assistant.io/integrations/sonos).
  - [x] Speech enhancement (does not work when playing music via roon) via [Sonos integration](https://www.home-assistant.io/integrations/sonos).
  - [x] Speaker group management via [Mini Media Player](https://github.com/kalkih/mini-media-player).
  - [x] Bass/Treble via [node-sonos-http-api](https://github.com/jishi/node-sonos-http-api).
  - [ ] Loudness.
    * Seems to be not possible yet.
  - [ ] Balance.
    * Seems to be not possible yet.
  - [ ] Volume level of rear speakers.
    * Seems to be not possible yet.
  - [x] Control subwoofer via [node-sonos-http-api](https://github.com/jishi/node-sonos-http-api).
    - [x] On/Off.
    - [x] Volume level.
    - [x] Crossover frequency.
    - [x] Polarity.
  - [x] Control status lights via [Sonos integration](https://www.home-assistant.io/integrations/sonos).
  - [x] Control buttons via [Sonos integration](https://www.home-assistant.io/integrations/sonos).
* **Roon**
  - [x] Control/Show info.
    - [x] [RoonLabs music player integration](https://www.home-assistant.io/integrations/roon/).
      - [ ] Transfer zones.
    - [ ] Remote control with [roon-cec-controller-extension](https://github.com/benjaminbellamy/roon-cec-controller-extension).
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
* **Android TV**
  - [x] Turn TV on via [Wake on LAN integration](https://www.home-assistant.io/integrations/wake_on_lan/).
  - [x] Turn TV off via [Android TV integration](https://www.home-assistant.io/integrations/androidtv/).
  - [x] Control TV.
    - [Android TV integration](https://www.home-assistant.io/integrations/androidtv/).
  - [x] [Notifications for Android TV / FireTV ](https://www.home-assistant.io/integrations/nfandroidtv/).
    - [ ] Not tested yet.
* **AVM FRITZ!Box**
  - [x] Show internet connectivity (with external IP and uptime attributes) via [AVM FRITZ!Box Tools integration](https://www.home-assistant.io/integrations/fritz/).
  - [x] Turn wifi and guest wifi on/off ([AVM FRITZ!Box Tools integration](https://www.home-assistant.io/integrations/fritz/).
* **AVM FRITZ!DECT devices**
  * Control.
    - [x] AVM FRITZ!DECT 200 (smart plug).
    - [x] AVM FRITZ!DECT 210 (smart plug).
    - [x] AVM FRITZ!DECT 300/Eurotronic Comet DECT (radiator control).
    - [ ] AVM FRITZ!DECT 400 (push button switch).
      * Currently not implemented in Home Assistant.
    - [ ] AVM FRITZ!DECT 440 (push button switch).
      * Currently not implemented in Home Assistant.
    - [ ] AVM FRITZ!DECT 500 (LED light).
      * Currently not implemented in Home Assistant.
    - [ ] Rademacher RolloTron DECT 1213 (shutter).
      * Currently not implemented in Home Assistant.
      - [ ] Close shutter when TV is turned on.
        * To avoid light glare.
      - [ ] Go to favorite position at a given time.
  * Show info
    - [x] Deutsche Telekom (Eurotronic) 40318684 (door/window contact).
    - [x] AVM FRITZ!DECT 200 (smart plug).
      - [x] Power consumption.
      - [x] Total power consumption.
    - [x] AVM FRITZ!DECT 210 (smart plug).
      - [x] Power Consumption.
      - [x] Total Power Consumption.
    - [x] AVM FRITZ!DECT 300/Eurotronic Comet DECT (radiator control).
      - [x] Battery level.
    - [ ] AVM FRITZ!DECT 400 (push button switch).
      - [x] Battery Level.
    - [x] AVM FRITZ!DECT 440 (push button switch).
      - [x] Temperature.
      - [x] Battery Level.
      - [ ] Humidity.
        * Currently not implemented in Home Assistant.
    - [x] Rademacher RolloTron DECT 1213 (shutter).
      * Shows only whether open or closed (even if only half open) - no intermediate levels.
* **Ecovacs Deebot** ([lovelace-xiaomi-vacuum-card](https://github.com/benct/lovelace-xiaomi-vacuum-card)).
  - [x] Control.
  - [x] Show info.
- [x] Cooking Timer.
* **Android** (Mobile/TV)
  - [x] Show info.
    - [x] Akku.
    - [x] Connectivity.
    - [x] Notifications/Messages.
    - [ ] Show Home Assistant notifications ([Notifications for Android TV / Fire TV ](https://www.home-assistant.io/integrations/nfandroidtv/)).
      * Not tested yet.
    - [x] State.

## ToDo/Ideas
- [ ] Make timer card more compact.
  - [ ] Show date.
- [ ] Child lock automation.
  - [ ] All buttons of Fritz!Dect devices off.
  - [ ] All buttons of Sonos devices off.
- [ ] Presence detection.
  - [ ] Music off.
  - [ ] All devices off.
- [ ] Show humidity of basement.

## Links

* https://github.com/christian-ek/home-assistant-config - a lot of inspiration, especially for Sonos.