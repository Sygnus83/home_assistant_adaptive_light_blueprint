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
