## App configuration

```yaml
sentry:
  module: sentry
  class: Sentry
  dsn: !secret sentry_dsn
  environment: optional
  release: optional
  traces_sample_rate: 1.0
```
