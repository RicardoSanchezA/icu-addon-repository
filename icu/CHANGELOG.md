# Changelog

## 0.5.0

- Add smart-plug/switch entity support: switches follow an area's lighting
  on/off state, with an optional per-area brightness threshold (reading the
  area's real light brightness from Home Assistant) that turns them off
  below a configurable percentage and back on once brightness recovers.

## 0.4.1

- Fix Supervisor discovery: the announced service now matches the Python
  integration's actual domain (`icu`, not `icu.engine`), so Home Assistant
  can route the discovery to it instead of logging an invalid-domain error.

## 0.4.0

- Add the `observer_mode` option: ICU computes and logs every lighting
  decision but never dispatches a real Home Assistant service call.

## 0.1.0

- Initial experimental package with Supervisor discovery.
