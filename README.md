### Adaptive Light Controller

A flexible, customizable Home Assistant blueprint that controls your lights based on lux (ambient light), with optional periodic updates, sunrise/sunset scheduling, cover conditions, and brightness-change filtering.

#### Key Features:
* **Lux-Based Dimming:** Automatically adjusts the brightness of target lights based on specified ambient light sensor values (with minimum and maximum thresholds).
* **Periodic Update:** Optionally allows light states to update at regular intervals (e.g., every minute) even if the light sensor value does not change.
* **Time-Based Scheduling:** Restricts operation exclusively to nighttime or daytime periods, with offsets relative to sunrise and sunset times.
* **Cover Conditions:** Allows you to specify one or more covers (blinds/shutters); the automation only runs if their position is above or below a given threshold.
* **Brightness Change Threshold:** Prevents unnecessary commands by only updating the light if the desired brightness change reaches a specified percentage.
* **Color and Color Temperature Management:** Supports fixed RGB colors, color temperatures specified in Kelvin, and out-of-range (over/under) value handling.
* **Manual Override:** The automation checks the state of your custom `input_boolean` helper at the start. If active, it pauses execution to protect your manual adjustments.
* **Night / Sleep Mode:** Uses a fixed, low `sleep_brightness` value and warm tones while ignoring lux levels when your sleep mode helper is enabled.
* **Circadian Color Temperature:** Continuously adjusts color temperature based on `sun.sun` elevation (warm at sunrise/sunset, cooler at noon).
* **Smart Presence Control:** Configurable presence hold time (`Presence Hold Time`) prevents sudden darkness during short pauses, while instant motion triggers (`Force Update on Motion`) update lights immediately without waiting for change thresholds.

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
* **Kézi felülbírálás (Manual Override):** Az automatika elején ellenőrzi az `input_boolean` segédkapcsoló állapotát; ha be van kapcsolva, leáll, így békén hagyja a manuális beállításokat.
* **Éjszakai / Alvás mód (Sleep Mode):** Aktív segédkapcsoló esetén figyelmen kívül hagyja a lux-értékeket, és egy fix, alacsony `sleep_brightness` fényerőt alkalmaz.
* **Cirkadián színhőmérséklet:** A `sun.sun` napmagassága (*elevation*) alapján folyamatosan hangolja a fényeket (napkeltekor/nyugtakor meleg, délben hűvösebb tónus).
* **Intelligens jelenlét-kezelés:** A beállítható tartási idő (`Presence Hold Time`) megakadályozza a hirtelen sötétedést, a mozgásra történő azonnali frissítés (`Force Update on Motion`) pedig küszöbértékek nélkül, késlekedés nélkül reagál.

---

## Beállítási példák / Felület:

<p align="center">
  <img width="700" alt="Blueprint beállítás 1" src="https://github.com/user-attachments/assets/cfec5a50-186c-4e35-bbae-009b55f04006" />
</p>

<p align="center">
  <img width="700" alt="Blueprint beállítás 2" src="https://github.com/user-attachments/assets/51f9363c-2a31-4f6e-a56f-f9832b1c419f" />
</p>

<p align="center">
  <img width="700" alt="Blueprint beállítás 3" src="https://github.com/user-attachments/assets/25ee803a-fb88-4ca1-af8b-6b9098dd6d03" />
</p>

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint URL](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fraw.githubusercontent.com%2FSygnus83%2Fhome_assistant_adaptive_light_blueprint%2Fmain%2Fblueprints%2Fautomation%2Fadaptive_light_controller.yaml)
