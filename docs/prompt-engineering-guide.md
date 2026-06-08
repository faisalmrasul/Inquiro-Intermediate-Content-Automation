# Prompt Engineering Guide for Multi-Format Content Repurposer

## Core Strategy

The LLM prompt is highly structured to ensure **reliable, parseable outputs** across platforms.

### System Prompt Highlights
- **Role**: Expert growth marketer + prompt engineer
- **Strict Format**: Uses `---PLATFORM---` delimiters
- **Platform Rules**:
  - LinkedIn: Authority + line breaks, no emojis
  - Twitter: 3-part thread with CTAs
  - Email: High curiosity, conversational
  - Instagram: Engaging + hashtags
  - YouTube: SEO title + description
- **Constraints**: Brand voice, length, CTA focus

### Advanced Prompt Techniques Used
1. **Delimiter-based parsing** (robust against minor variations)
2. **Few-shot style instructions** via detailed rules
3. **Negative prompting** ("no extra text")
4. **Temperature control** (recommended 0.7 in Groq node)

### Tips to Iterate
- Add **few-shot examples** (good output samples) inside the system message for better consistency.
- Use **JSON mode** if switching to models that support it.
- Test with different Groq models (`llama-3.3-70b-versatile` performs best).

Full prompt is inside the **Multi-Format LLM Chain** node.
