# Future Personas Chat | 未来人物谈

> ⚠️ **Bring Your Own API Key**: This is a frontend-only HTML app. You need to configure your own DeepSeek or OpenAI-compatible API key to use it.
>
> An AI roleplay chatroom based on 2035 future personas, supporting 1v1 chat, group debate, and Prompt Lab debugging.

---

## Origin

This is a "future personas chatroom" built for my own needs.

When doing Futures Design / Speculative Design, I wanted "living" references—not static reports, but future characters you can talk to, argue with, and have unexpected collisions of ideas. So I created this project: 10 characters from different fields in 2035, injected with real future trend signals, making them "future residents" you can chat with.

**Disclaimer**: These personas provide **inspiration without reference value**—they are fictional, biased, and imagined. Treat them as "creative catalysts," not predictions.

---

## Features

### 🤖 1v1 Chat
Choose any persona for a one-on-one deep conversation. Each persona has:
- Unique identity background and career trajectory
- Personalized speaking style (colloquial, emotional, informal)
- Memory and opinions based on real trend signals
- Long-term memory (context preserved across conversations)

### 👥 Group Chat Mode
Support multiple personas debating or brainstorming simultaneously:
- **Debate Mode**: Set a topic and watch how different stances clash
- **Brainstorm Mode**: Gather diverse perspectives around a theme
- Personas will naturally respond to each other, forming organic conversation flow

### 🧪 Prompt Lab v3
A built-in prompt engineering lab for assembling and debugging persona profiles:
- **Layered prompt structure**: Identity → Speech → Worldview → Narrative Reference → Memory → Attitude
- **Framework switching**: Supports CO-STAR, Few-Shot, RFT, Ontology, Attack-Hardened, and more
- **Wind tunnel testing**: Real-time validation of prompt effects, checking narrative length, formal language, stage directions, etc.
- **Custom personas**: Create your own 2035 residents from scratch

---

## Technical Setup

### Prompt Structure (8-9 Layers)

Each persona is assembled from 8-9 prompt layers:

| Layer | Content | Purpose |
|-------|---------|---------|
| 1 | Absolute Identity Rules | Hard constraints to prevent role drift |
| 2 | Who You Are | Core identity and current state |
| 3 | How You Speak | Speech patterns, catchphrases, emotional expression |
| 4 | Example Tone | 2-6 paragraphs of authentic dialogue samples |
| 5 | World Premise | 2035 technology/society/culture context |
| 6 | Inner Tension Points | Character's internal contradictions and struggles |
| 7 | Policy Levers | Social issues relevant to the character |
| 8 | Career Background (reference, not current state) | Key experiences (demoted to reference layer to prevent repetitive narration) |
| 9 | Your Attitude | Default response style to users |

**Anti-Narrative Constraint**: All personas have explicit constraints—do not repeat specific events from your backstory unless the user directly asks. Daily life is fluid, not fixed to a single day.

### Future Trend Signal Injection

I extracted key signals from a future trends document and injected them into personas' memory settings:
- Technology trends (AI, climate tech, bioengineering)
- Social trends (demographics, work patterns, cultural shifts)
- Policy trends (regulatory frameworks, international agreements, geopolitics)

These signals are not background decoration—they are "real events" the characters have experienced or are experiencing.

### Model Support

- **Default**: DeepSeek-V4-Flash (cost-effective, fast response)
- **Compatible**: Any OpenAI-format API (OpenAI, Azure, custom endpoints, etc.)
- Configure API Key and Base URL in the settings panel to switch

---

## Persona List (10 Residents of 2035)

| Persona | Identity | Keywords |
|---------|----------|----------|
| 周维 (Zhou Wei) | Former big tech programmer, now community digital nomad | Tech critique, low-power living |
| Naomi | Climate refugee descendant, carbon trading lawyer | Environmental justice, intergenerational trauma |
| 林一舟 (Lin Yizhou) | Retired esports player, neural interface experiencer | Virtual identity, body modification |
| 阮氏梅 (Nguyen Thi Mai) | Vietnamese, global supply chain coordinator | Geopolitical mobility, cultural in-between |
| Omar Al-Farsi | Middle Eastern data archaeologist | Digital heritage, historical reconstruction |
| 赵晓萌 (Zhao Xiaomeng) | Rural education tech volunteer | Education equity, tech accessibility |
| 陈默 (Chen Mo) | Former journalist, deepfake investigator | Information authenticity, trust crisis |
| Helena | Nordic biohacker, longevity community member | Body sovereignty, aging ethics |
| Clara | African open-source agricultural AI developer | Tech colonialism, knowledge sharing |
| 老周 (Lao Zhou) | Retired taxi driver, urban memory guardian | Oral history, technological forgetting |

---

## Quick Start

1. Download `finance-personas-chat-v5-通用版.html`, open it directly in your browser (no server, no installation)
2. Configure your API Key in settings (DeepSeek or other OpenAI-compatible service)
3. Choose a persona and start chatting
4. Try group chat mode and see how personas interact
5. Enter Prompt Lab to debug or create your own characters

> 💡 **Tip**: This is a pure frontend single-file app. All data (including API Key) is stored only in your browser locally and never uploaded to any server.

---

## File Structure

```
final/
├── finance-personas-chat-v5-通用版.html    # Main app (single file, open directly)
└── v5_通用版_测试报告.md                    # Persona test report
```

> This is a **single-file HTML app** with no build steps, no dependency installation—just open in browser and run.

---

## Version History

- **v5 General** (current): Removed finance/scenario dual versions, focused on 2035 general personas; optimized prompt structure (speechStyle promoted, narrative demoted); added anti-narrative constraints; Prompt Lab v3
- v4: Finance edition + original 2035 dual versions, tech disruption/failure scenario modes
- v1-v3: Early prototypes, gradually added group chat, memory, Prompt Lab, etc.

---

## Acknowledgments

- Inspiration: Stuart Candy's "Experiential Futures", Jane McGonigal's "Future Simulation"
- Trend signals reference: Public reports from multiple futures research institutions
- Model support: DeepSeek, OpenAI

---

*"The future is not a place we are going to, but something we are creating."—These personas are just the starting point; the real future is written by you and them.*
