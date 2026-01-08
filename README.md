# langbreak

![Example file](/example.png)

A lightweight bash script that displays a coloured language breakdown bar for your codebase, similar to GitHub's linguist feature.

# Installation

```bash
# download the script
chmod +x langbreak
```

# Usage

## Basic Usage
Display a visual breakdown of the current directory:
```bash
./langbreak
```

## Help
```bash
./langbreak --help
```

## Options
Export language data to JSON or YAML:
```bash
./langbreak --json
./langbreak --yaml
```

Redirect to a file:
```bash
./langbreak --json > stats.json
./langbreak --yaml > stats.yaml
```

### JSON Export
```json
{
  "timestamp": "2026-01-08T18:34:27+00:00",
  "total_bytes": 15234,
  "languages": [
    {
      "name": "Python",
      "bytes": 8500,
      "files": 12,
      "percentage": 55.8
    }
  ]
}
```

### YAML Export
```yaml
timestamp: "2026-01-08T18:34:27+00:00"
total_bytes: 15234
languages:
  - name: "Python"
    bytes: 8500
    files: 12
    percentage: 55.8
```

# License

GPLv3
