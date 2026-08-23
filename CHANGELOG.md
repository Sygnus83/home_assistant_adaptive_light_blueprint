# Changelog


## [1.0.0] - 2026-07-25 *(Initial Release)*

### Added
- Initial release of the **Adaptive Light Controller** blueprint.
- Lux-based dynamic dimming matching ambient light sensor values.
- Optional trigger light support to execute automation when specific lights turn on.
- Periodic updates with configurable minute intervals.
- Sun schedule options (Run from sunset to sunrise or sunrise to sunset) with custom sunrise/sunset offsets.
- Cover condition integration to limit execution based on roller shutter/blind positions (above/below thresholds).
- Advanced brightness range handling (behavior when ambient light is over max or under min limits).
- Color temperature (Kelvin) and RGB color adaptation settings (both standard and outside range).
- Minimum brightness change threshold to prevent spamming unnecessary light updates.
- Configurable transition time for smooth dimming.
  
### Hozzáadva
- Az Adaptive Light Controller blueprint első kiadása.
- Lux-alapú, dinamikus fényerőszabályzás a környezeti fényszenzor értékei alapján.
- Opcionális triggerlámpa-támogatás: az automatizmus megadott lámpák bekapcsolásakor is elindul.
- Rendszeres frissítés állítható perces időközökkel.
- Napkelte-/napnyugta-időzítés: napnyugtától napkeltéig vagy napkeltétől napnyugtáig, egyedi eltolásokkal.
- Redőnyfeltétel a futás korlátozására redőny- vagy árnyékolópozíció alapján, állítható küszöbérték felett vagy alatt.
- Haladó fényerőtartomány-kezelés a minimum- vagy maximális környezeti fényértéken kívüli működéshez.
- Kelvin színhőmérséklet- és RGB-színbeállítások, normál és tartományon kívüli helyzetekre is.
- Minimális fényerőváltozási küszöb a felesleges lámpafrissítések elkerülésére.
- Állítható átmeneti idő a fokozatos fényerőváltáshoz.

## [1.1.0] - 2026-08-23 

### Added
- Version number included in the blueprint name and description.
- Optional presence/motion-based brightness control: normal lux-based operation when presence is detected,
  specified fixed brightness when no presence is detected.
- State changes of the selected presence or motion sensors immediately trigger a brightness update.
- Optional fixed fallback brightness if the lux sensor state is unknown or unavailable.
### Fixed
- Regular updates migrated to a proper time_pattern trigger.
- Update interval now selectable between 1 to 10 minutes with reliable minute-based scheduling.

### Hozzáadva  
- Verziószám megjelenítése a blueprint nevében és leírásában.
- Opcionális jelenlét-/mozgásalapú fényerőszabályzás:
  - érzékelt jelenlétnél normál lux-alapú működés;
  - jelenlét hiányában megadott fix fényerő.
- A kiválasztott jelenlét- vagy mozgásérzékelő állapotváltozása azonnal frissíti a fényerőt.
- Opcionális fix tartalékfényerő, ha a luxszenzor állapota unknown vagy unavailable.  
### Javítva
- A rendszeres frissítés valódi time_pattern triggerre változott.
- A frissítési időköz most 1–10 perc között választható, megbízható perces ütemezéssel.

