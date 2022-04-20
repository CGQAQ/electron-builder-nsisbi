# electron-builder-nsisbi
nsisbi for electron-builder customNsisBinary


In your electron-builder config

```json
"build": {
  "nsis": {
    "include": "nsis/installer.nsh",
    "customNsisBinary": {
      "url": "https://github.com/CGQAQ/electron-builder-nsisbi/releases/download/nsis-1.0.0/nsis-1.0.0.7z",
      "version": "1.0.0",
      "checksum": "5qFkDRwmXEVdRRrwSFhIYfzsiNFeimFMIvzZUd3tzgT3osMnNiuuXhvLT7vPkLKvFFoOC81TbOoNlVjfBJoQYw=="
    }
  }
}
```

in your nsis/installer.nsh

add
```nsis
OutFileMode data
```
