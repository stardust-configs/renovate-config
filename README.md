# @stardust-configs/renovate-config

> Shareable Renovate config

## Usage

Edit `renovate.json`.

```json
{
  "extends": ["@stardust-configs"]
}
```

## Presets

### `base` preset

- Immediately update

```json
{
  "extends": ["@stardust-configs/renovate-config:base"]
}
```

### `app` preset

- Weekly update
- Grouping devDependencies and dependencies

```json
{
  "extends": ["@stardust-configs/renovate-config:app"]
}
```

### `lib` preset

- Monthly update
- Automerge non-major minor updates, non-major patch updates

```json
{
  "extends": ["@stardust-configs/renovate-config:lib"]
}
```
