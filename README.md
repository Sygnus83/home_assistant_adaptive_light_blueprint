
---

### Adaptive Light Controller

A flexible, customizable Home Assistant blueprint that controls your lights based on lux (ambient light), with optional periodic updates, sunrise/sunset scheduling, cover conditions, and brightness-change filtering.

#### Key Features:
* **Lux-Based Dimming:** Automatically adjusts the brightness of target lights based on specified ambient light sensor values (with minimum and maximum thresholds).
* **Periodic Update:** Optionally allows light states to update at regular intervals (e.g., every minute) even if the light sensor value does not change.
* **Time-Based Scheduling:** Restricts operation exclusively to nighttime or daytime periods, with offsets relative to sunrise and sunset times.
* **Cover Conditions:** Allows you to specify one or more covers (blinds/shutters); the automation only runs if their position is above or below a given threshold.
* **Brightness Change Threshold:** Prevents unnecessary commands by only updating the light if the desired brightness change reaches a specified percentage.
* **Color and Color Temperature Management:** Supports fixed RGB colors, color temperatures specified in Kelvin, and out-of-range (over/under) value handling.


---

### Adaptive Light Controller (Adaptív Fényvezérlő)

Egy rugalmas, személyre szabható Home Assistant blueprint, amely lux (fényerő) alapon, opcionális időzítésekkel, napkelte/naplemente szabályozással, redőny-feltételekkel és fényerő-változási szűréssel vezérli a lámpáidat.

#### Főbb jellemzők:
* **Lux-alapú dimmelés:** Automatikusan beállítja a célfények fényerejét a megadott környezeti fényérzékelő értékei alapján (minimum és maximum küszöbökkel).
* **Időszakos frissítés (Periodic Update):** Opcionálisan beállítható, hogy a lámpák állapota rendszeres időközönként (pl. percenként) frissüljön akkor is, ha a fényérzékelő értéke nem változik.
* **Napszakhoz kötött ütemezés:** Korlátozható a működés kizárólag éjszakai vagy nappali időszakra, eltolásokkal (offset) a napkelte és naplemente időpontjaihoz képest.
* **Redőnyök szerinti feltétel:** Megadhatsz egy vagy több redőnyt; a vezérlés csak akkor fut le, ha azok pozíciója egy adott küszöb alatt vagy felett van.
* **Fényerő-változási küszöb:** Megakadályozza a felesleges parancsok küldését azáltal, hogy csak akkor frissíti a lámpát, ha a kívánt fényerő változása eléri a megadott százalékos értéket.
* **Szín- és színhőmérséklet-kezelés:** Lehetőség van fix RGB szín, Kelvinben megadott színhőmérséklet, valamint a tartományon kívüli (over/under) értékek megadására is.


[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint URL](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fraw.githubusercontent.com%2FSygnus83%2Fhome_assistant_adaptive_light_blueprint%2Fmain%2Fblueprints%2Fautomation%2Fadaptive_light_controller.yaml)
