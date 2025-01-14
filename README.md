# blueprint-auto-luftreiniger v1.1

📘Dieser Blueprint schaltet (mehrere) Luftreiniger nach Entität, Schalter oder Schalter am Gerät ein und automatisch nach eingestelltem Luftwert wieder aus. Zeitversatz nachdem die Aktion ausgeführt wird liegt bei 3min.

🎛️ Schalter oder Entität: Luftreiniger wird nach Schalter oder Entität eingeschaltet und nach gesetztem Luftwert automatisch wieder abgeschaltet. 

📅 Bereiche in denen Luftreiniger stehen können ausgewählt werden (Mehrfachauswahl an Luftreinigern mögl.)

⏰ Automatische Abschaltung: Luftreiniger wird nach gesetztem Luftwert und manueller Auslösung am Gerät automatisch wieder abgeschaltet.

<a href="https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fraw.githubusercontent.com%2Fjayjojayson%2Fblueprint-auto-luftreiniger%2Fmain%2FLuftreiniger-ausschalten-bei-bestimmten-Luftwert.yaml"><img width="250" alt="blueprint" src="https://github.com/user-attachments/assets/fa01530a-1d52-4b2b-b637-1269bd0cd747"></a>

#
Hi, today I would like to introduce you my first blueprint. It is certainly nothing special, but it has give me a chance to get to grips with the subject and I can conveniently control and switch on my air purifiers now. I use it for my Starkvind air purifier. The Blueprint Notes are in German, but I think it is self-explaining.

Our air purifier is often switched on manually by people in our household who know how to do it, and I wanted an option for automatic shutdown. :wink:

Should work with any air purifier and an air sensor for PPM. The sensors are built into the air purifier in the Starkvind things, so I built in a small offset of 3 minutes so that the correct air value can be determined first before the action starts.

Description of the blueprint:

:blue_book:This blueprint switches the air purifier on according to an entity, switch or switch on the device and automatically switches it off after the air value has been set. The time delay after the action is carried out is 3 minutes.

:control_knobs: Switch or entity: Air purifier is switched on according to a switch or entity and automatically switches it off again after the air value has been set.

:date: Areas in which air purifiers are located can be selected (multiple selection of air purifiers possible)*

:alarm_clock: Automatic switch-off: Air purifier is automatically switched off again after the air value has been set and manually triggered on the device.

<a href="https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fraw.githubusercontent.com%2Fjayjojayson%2Fblueprint-auto-luftreiniger%2Fmain%2FLuftreiniger-ausschalten-bei-bestimmten-Luftwert.yaml"><img width="250" alt="blueprint" src="https://github.com/user-attachments/assets/fa01530a-1d52-4b2b-b637-1269bd0cd747"></a>
