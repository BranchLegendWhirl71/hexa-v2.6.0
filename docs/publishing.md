# Publishing checklist

## 1. Repository

- **Name:** `hexa`
- **Description:** Memory scanner and editor for Windows x64 - fast scans, pointer paths, Lua console.
- **Topics:** `memory-scanner memory-editor reverse-engineering lua windows cpp debugging`
- **Visibility:** public

## 2. First push

```bash
git init
git add .
git commit -m "Hexa 2.6.0 - initial release"
git branch -M main
git remote add origin https://github.com/<you>/hexa.git
git push -u origin main
```

## 3. Release

1. Draft a release tagged `v2.6.0`.
2. Title: `Hexa 2.6.0`.
3. Body: copy the top entry from `CHANGELOG.md`.
4. Attach the build archive.
5. Publish.

## 4. Settings

| Setting | Value |
| --- | --- |
| Website | the download folder |
| Discussions | enabled |
| Issues | enabled |
| Social preview | export `assets/hero.svg` at 1280x640 |

## 5. First week

- [ ] Release + pin
- [ ] Push a small follow-up commit
- [ ] Reply to every issue within 24 h
- [ ] Publish one screenshot or clip
- [ ] Ship 2.6.0 patch with a visible fix

Keep a 2-3 day commit cadence. Consistency beats volume.