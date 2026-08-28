# Digital Garden community plugins

The community plugin registry for [Digital Garden](https://github.com/oleeskild/digitalgarden). The Obsidian plugin's **Plugins → Browse community plugins** gallery is driven by `community-plugins.json` in this repo.

## Submit your plugin

1. Publish your plugin as a public GitHub repo with `garden-plugin.json` at the root and a tagged release. See the [plugin author guide](https://github.com/oleeskild/digitalgarden/blob/main/docs/PLUGINS.md).
2. Open a pull request adding one entry to `community-plugins.json`:

```json
{
  "id": "your-plugin-id",
  "name": "Your Plugin",
  "author": "You",
  "description": "One sentence on what it does.",
  "repo": "you/garden-plugin-your-plugin",
  "screenshot": "screenshot.png"
}
```

`id` must match your manifest's id; `screenshot` (optional) is a path inside your repo. The registry is a directory, not an endorsement — users are warned that plugins run code in their site build.
