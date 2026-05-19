# Quick Reference: Telegram Bot Commands

## 🤖 Model Switching

Switch between your three configured LLM providers:

| Command | Model | Cost | Best For |
|---------|-------|------|----------|
| `/model deepseek` | DeepSeek 4 | ⭐ Cheapest | **DEFAULT** - Reasoning, code, writing |
| `/model claude` | Claude Sonnet 4.5 | 💎 Premium | Complex analysis, edge cases |
| `/model gemini` | Gemini 2.0 Flash | ⚡ Fastest | Speed-critical tasks, coding |

**Example:**
```
User: /model deepseek
Bot: ✅ Model switched to deepseek-reasoner
```

---

## 💬 Skill Triggers

Your installed skills activate automatically or via keywords:

### Website Intelligence
- "Build a website for [business]"
- "Scrape and rebuild [URL]"
- "Competitive analysis for [niche]"
- "Website audit"

### 3D Animation Creator
- "Create a scroll-stop animation"
- "Apple-style scroll video"
- Upload a video file + "Make it scroll-driven"

### NotebookLM
- "Create a podcast about [topic]"
- "Generate a quiz from [sources]"
- "Summarize these URLs"
- "Turn this into flashcards"

---

## 📊 Cost Per Task (Rough Estimates)

Using **DeepSeek 4** (default):

| Task | Tokens | Cost |
|------|--------|------|
| Quick reply | 200-500 | $0.0003 - $0.0015 |
| Code generation | 1,000-2,000 | $0.0015 - $0.004 |
| Full document | 5,000-10,000 | $0.01 - $0.02 |
| Website intelligence flow | 20,000-50,000 | $0.03 - $0.10 |

---

## 🚀 Speed Tips

- **Fastest response:** `/model gemini`
- **Best reasoning:** `/model claude`
- **Best value:** `/model deepseek` (current default)

For website design tasks, **stay with DeepSeek** — you'll save ~$100+/month vs Claude Sonnet.

---

## 🔔 Reminders

- **3 providers configured:** No setup needed, just switch via `/model`
- **Telegram bot is live:** 24/7 access to Hermes
- **User ID restricted:** Only you (6541358599) can access the bot
- **Default model:** DeepSeek 4 (cost-optimized)

---

**Status:** ✅ Ready to use  
**Config location:** `/home/hermeswebui/.hermes/config.yaml`
