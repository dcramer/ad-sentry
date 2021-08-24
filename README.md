# Sentry for AppDaemon

Load this repository in HACS and configure the Sentry module in ypur `apps.yaml`:

```yaml
global_modules:
  - sentry

sentry:
  module: sentry
  class: Sentry
  dsn: !secret sentry_dsn
```

Additionally you need to add the contents of `apps/requirement.txt` to your master `requirements.txt` file, located in the `apps/` root next to your `apps.yaml`.

If you are using Home Assistant Core (Hass.io) you will need to add the requirements in the Add-on configuration. For example:

```json
{
  "log_level": "info",
  "system_packages": [],
  "python_packages": ["sentry-sdk"]
}
```
