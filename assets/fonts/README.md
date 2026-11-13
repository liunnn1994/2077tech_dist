# Chinese text atlas

`NotoSansSC.png` and `NotoSansSC.json` are an MSDF atlas of the characters used by
`src/config/i18n.ts`, plus printable ASCII. They use Noto Sans CJK SC Medium under
the adjacent SIL Open Font License. English text keeps the existing IBM Plex Mono
atlas; the combined temperature label and number mesh uses Noto in both languages.

Source: https://github.com/notofonts/noto-cjk/blob/main/Sans/OTF/SimplifiedChinese/NotoSansCJKsc-Medium.otf

After adding Chinese characters, regenerate with msdf-atlas-gen 1.4:

```powershell
node scripts/check-i18n.ts <path-to-msdf-atlas-gen.exe> <path-to-NotoSansCJKsc-Medium.otf>
```

Run `node scripts/check-i18n.ts` to check glyph coverage and language defaults.
