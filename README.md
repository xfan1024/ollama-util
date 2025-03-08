# ollama-util

A command-line tool for managing Ollama model repositories and transfer operations.

## Usage

### Basic Commands

```bash
# List models
ollama-util --ollama-dir /path/to/ollama ls

# Copy model
ollama-util --ollama-dir /source cp model:tag --to /destination

# Move model
ollama-util --ollama-dir /source mv model:tag --to /destination
```

### Command Options

| Argument       | Description                               |
| :------------- | :---------------------------------------- |
| `--ollama-dir` | Base directory containing Ollama models   |
| `--to`         | Target directory for copy/move operations |

## Examples

### List Models

```
ollama-util --ollama-dir ~/ollama list
```

### Transfer Model

```
ollama-util --ollama-dir /path/to/old-ollama-dir mv deepseek-r1:32b --to /path/to/new-ollama-dir
```

## Development Background

- **AI-Generated Content**
  This tool and documentation were generated by deepseek-r1:167b through collaborative development with xfan1024.
- **Experimental Status**
  This is experimental software. Verify critical operations and test thoroughly before production use.
- **Error Reporting**
  Found an issue? Please:
  1. Submit via GitHub Issues
  2. Create Pull Request for fixes
  3. Include reproduction steps and environment details

