# AI-Keys

A VSCode extension to use and manage AI from varied sources.

Keep control of your keys, usage and costs directly to the model provider.

![AI-Keys Demo](https://github.com/tomcodedthis/AI-Keys/blob/main/images/aikeys-demo.gif?raw=true)

---

## Features

**Inline**
Focus your prompt line, then press `CMD/CTRL + Shift + ?`

**Input Box**
`CMD/CTRL + Shift + P` and search for `AI-Keys: Search Prompt`

Specify model (default is customizable):

```python
gbt tell a joke
```

```python
codex write a function that adds 2 numbers
```

```python
dalle an image of a smiling dog
```

- Shorthand configuration (convert / optimise / explain):

```python
cv javascript def add(x, y) return x + y

# convert javascript 
# def add(x, y):
#   return x + y
```

```typescript
op def add(x, y) return x + y

// optimise
// function add(x, y) {
//   return x + y
// }
```

```python
ex def add(x, y) return x + y

# explain
# def add(x, y):
#   return x + y`
```

---

## Usage

Multiline prompts are currently only supported for **comments**

**Setup**
`CMD/CTRL + Shift + P` and search for `AI-Keys: Open Settings`

- Set API Keys and default configuration:
![AI-Keys Settings](https://github.com/tomcodedthis/AI-Keys/blob/main/images/aikeys-settings.png?raw=true)

---

| Model  | Prefix | Example |
| ------ | ------ | ------- |
| GBT-3  | `gbt` / `gbt3` | `gbt what is ai model gbt3` |
| | | `gbt3 what is ai model gbt` |
| Codex  | `codex` | `codex write a function that sums an array of numbers` |
| DALL·E | `dalle` | `dalle a smiling dog` |

| Argumment | Examples | Description
| ---------- | ----------- | -------- |
| optimise/ze | `optimise` / `gbt3 op` | Optimise prompt |
| convert | `cv python` / `codex cv typescript` | Convert prompt to specified language |
| explain | `explain` / `gbt3 ex` | Explain prompt |
---

## Requirements

Atleast one API key from our supported AI providers:

### [OpenAI](https://platform.openai.com/account/api-keys)

GBT-3 (text-generation: low-cost but more accurate)
Codex (code-generation: free)
DALL·E (imgage-generation: higher-cost)

---

## Extension Settings

- `aikeys.goToSettings`: Open extension settings
- `aikeys.sendLinePrompt`: Send prompts from inline active editor
- `aikeys.sendBoxPrompt`: Send prompts from VSCode input box

---

## Known Issues

Please raise any issues / suggestions

### To-Do

Contributions are widely encouraged, get involved to earn XP

- Write proper tests for pre-release checks
- Stream response [info](https://github.com/openai/openai-node/issues/18)
- More models/provider integrations
- More types of generation (tts, video, 3d models)
- Add auto completion for arguments
- Support for fine-tuned models
- More-configuration options:
  - Train own models

---

## In-Development

Features currently being worked on:

- Multiple providers (Google, rev.ai)
- Storing secret API keys
- More configuration options

---

## Release Notes

### 0.0.1

Initial release of AIKeys
