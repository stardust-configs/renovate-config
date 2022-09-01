# @stardust-configs/renovate-config

> Shareable Renovate config

## Usage

Edit `renovate.json`.

<details>
<summary><code>app</code> preset</summary>

> for Application

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>stardust-configs/renovate-config:app"]
}
```

- Pin all dependencies (Except peerDependencies)
- Monthly update
- Grouping non-major dependencies updates, non-major devDependencies updates

</details>

<details>
<summary><code>lib</code> preset</summary>

> for Library (Browser & Node.js)

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>stardust-configs/renovate-config:lib"]
}
```

- Pin only devDependencies
- Monthly update
- Automerge non-major updates

</details>

<details>
<summary><code>libNode</code> preset</summary>

> for Library (Node.js)

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>stardust-configs/renovate-config:libNode"]
}
```

- Pin all dependencies (Except peerDependencies)
- Monthly update
- Automerge non-major updates

</details>

## Override

Override `renovate.json`.

<details>
<summary><code>label</code> preset</summary>

```json
{
  "extends": [":label(dependencies)"]
}
```

</details>

<details>
<summary><code>assignee</code> preset</summary>

```json
{
  "extends": [":assignee(p-chan)"]
}
```

</details>

## FAQ

### Why does each preset have a different target to pin?

See [Should you Pin your JavaScript Dependencies?](https://docs.renovatebot.com/dependency-pinning/#so-whats-best).

### Why does the non-major rules exclude v0.x?

Because during `v0.x`, even non-major updates cause breaking changes.

## Author

[@p-chan](https://github.com/p-chan)

## LICENSE

MIT
