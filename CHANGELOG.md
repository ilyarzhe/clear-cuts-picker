# Changelog

## [0.0.0.3] - 2026-08-12

### Changed
- Echo the `nonce` from the URL fragment back to the extension in every
  `pickerAuthRequest` / `pickerResult` message. Required by extension v2.7.3.0+
  trust-boundary hardening — the extension fails closed on requests without a
  valid nonce. Old extensions ignore the extra field, so this deploy is safe
  before the extension update.

## [0.0.0.2] - 2026-05-27

### Added
- Wire `appId` parameter to `PickerBuilder.setAppId()` for proper Google Picker OAuth scoping

## [0.0.0.1] - 2026-05-27

### Added
- Extract `appId` URL parameter from query string for Chrome extension consumption