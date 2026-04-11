# Install — Gemini

> **Recommended**: Run `./install.sh --agent=gemini-cli` from the repo root for automated installation.
> The manual steps below are for reference or troubleshooting.

## Quick install

Paste the contents of `cognitive-protocol.md` into the `system_instruction` field of your Gemini API call or Google AI Studio system prompt.

将 `cognitive-protocol.md` 的内容粘贴到 Gemini API 调用的 `system_instruction` 字段或 Google AI Studio 系统提示词中。

## API example

```python
import google.generativeai as genai

# Read the cognitive protocol
with open("cognitive-protocol.md", "r") as f:
    dialectical_protocol = f.read()

model = genai.GenerativeModel(
    model_name="gemini-2.5-pro",
    system_instruction=dialectical_protocol
)

response = model.generate_content("Your prompt here")
```

## Google AI Studio

1. Open Google AI Studio
2. Click "System Instructions"
3. Paste the full contents of `cognitive-protocol.md`
4. The protocol activates for all conversations in that session

## Verify

Ask Gemini: "What dialectical thinking rules are you following?" It should list: contradiction network mapping, principal contradiction location, nature judgment, transformation monitoring, steel-manning, concrete analysis of concrete conditions.

## Notes

- `cognitive-protocol.md` is ~30 lines — minimal token overhead.
- For full reference, include `SKILL.md` content in the system instruction or as context when deeper analysis is needed.
