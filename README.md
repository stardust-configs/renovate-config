# @stardust-configs/renovate-config

> Shareable Renovate config

## Usage

Edit `renovate.json`.

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["@stardust-configs"]
}
```

## Presets

### `base` preset

- Immediately update

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["@stardust-configs/renovate-config:base"]
}
```

### `app` preset

- Weekly update
- Grouping devDependencies and dependencies

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["@stardust-configs/renovate-config:app"]
}
```

### `lib` preset

- Monthly update
- Automerge non-major minor updates, non-major patch updates

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["@stardust-configs/renovate-config:lib"]
}
```
