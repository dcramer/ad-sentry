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
