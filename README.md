## 📥 How to Use

To use this bucket with Scoop:

```powershell
scoop bucket add scoop-tools https://github.com/xuwenbolan/scoop-tools-bucket
```

Then you can install apps like this:

```powershell
scoop install app-name
```

For example:

```powershell
scoop install synclink
```

## 📂 Manifest Format

All manifest files are stored in the `bucket/` folder. Each file is a JSON that describes the app, similar to this:

```json
{
  "version": "1.0.0",
  "description": "An example tool.",
  "homepage": "https://example.com",
  "url": "https://example.com/tool.zip",
  "hash": "sha256:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "bin": "tool.exe",
  "shortcuts": [
    [
      "tool.exe",
      "Example Tool"
    ]
  ]
}
```

## 🤝 Contributing

Want to contribute?

- Fork the repo and add your JSON under the `bucket/` folder.
- Then make a Pull Request!
- Please follow the JSON format used in other manifests.

Alternatively, if you're a team member, ask to be added as a collaborator.

## 🛠 Tools

You can validate your manifest file using:

```powershell
scoop install scoop-format
scoop-format validate bucket/your-app.json
```
