# Telegram Bot Model Optimization

## Current Configuration (Cost-First Strategy)

**Default Model:** DeepSeek 4 (deepseek-reasoner)  
**Provider:** DeepSeek  
**Strategy:** Cheapest option for all tasks

---

## 💰 Cost Comparison (as of May 2026)

| Model | Provider | Input Cost | Output Cost | Best For |
|-------|----------|-----------|-----------|----------|
| **DeepSeek 4** ⭐ | DeepSeek | $0.55/M tokens | $2.19/M tokens | **DEFAULT - Everything (cheapest)** |
| Claude Haiku | Anthropic | $0.80/M tokens | $4.00/M tokens | Quick tasks (when cost not critical) |
| Claude Sonnet | Anthropic | $3.00/M tokens | $15.00/M tokens | Complex reasoning (premium) |
| Gemini 2.0 Flash | Google | $0.075/M tokens | $0.30/M tokens | Coding, speed (if token limits OK) |

---

## 🔧 How to Switch Models in Telegram

Your Telegram bot supports **runtime model switching** via the `/model` command:

### Usage

Send this to the bot:
```
/model deepseek
```

Available options:
- `/model deepseek` → Switch to DeepSeek 4 (default, cheapest) ⭐
- `/model claude` → Switch to Claude Sonnet 4.5 (best quality)
- `/model gemini` → Switch to Gemini 2.0 Flash (fastest)

The bot will confirm:
```
✅ Model switched to deepseek-reasoner
Provider: DeepSeek
Next message will use this model.
```

---

## 📊 Cost Breakdown by Task Type

Since you're on **cost-first strategy**, DeepSeek is optimal for all these. But here's the breakdown if you need to switch:

### Cheap Tasks (DeepSeek is perfect)
- Quick Q&A
- Summarization
- Brainstorming
- Simple writing
- Code explanation

**Cost per task:** ~$0.001 - $0.005

### Medium Tasks (DeepSeek still good)
- Code generation
- Detailed analysis
- Content creation
- Skill-based work

**Cost per task:** ~$0.01 - $0.10

### Expensive Tasks (Consider switching to Gemini or Claude if needed)
- Complex reasoning chains
- Multi-step problem solving
- Deep research synthesis
- Competitive intelligence analysis (website-intelligence skill)

**Cost per task:** ~$0.10 - $1.00

---

## 🎯 Recommended Strategy for Your Workflow

### For RG Revenue Website Business:

**Daily Use (Telegram):**
- **Default: DeepSeek 4** ✅ (cheapest, excellent reasoning)
- Cost savings: ~50% vs Claude Sonnet

**Premium Tasks (when quality > cost):**
- `website-intelligence` skill → Switch to `/model claude` (better for complex competitive analysis)
- `3d-animation-creator` → Stay with DeepSeek (great for code gen)
- `notebooklm` research → DeepSeek is fine (GPT-class reasoning)

**Time-Critical:**
- `/model gemini` for instant responses (marginally faster)

---

## 💡 Cost Optimization Tips

1. **Use DeepSeek by default** (already configured) ✅
2. **Only switch for complex tasks** where quality matters more than cost
3. **Monitor token usage** — longer prompts = higher costs
4. **Batch similar requests** to reduce overhead
5. **Use skills** (website-intelligence, 3d-animation-creator, etc.) — they're more efficient than conversational mode

---

## 🔐 API Keys Configured

All three providers are set up in `.env`:

| Provider | Status | Key Location |
|----------|--------|--------------|
| DeepSeek | ✅ Active | `DEEPSEEK_API_TOKEN` |
| Anthropic (Claude) | ✅ Active | `ANTHROPIC_API_KEY` |
| Google (Gemini) | ✅ Active | `GOOGLE_API_KEY` |

---

## 📈 Expected Monthly Costs (Rough Estimate)

Assuming **100 messages/day** on Telegram with average 500 input + 500 output tokens:

| Model | Daily Cost | Monthly Cost |
|-------|-----------|--------------|
| DeepSeek 4 (current) | ~$0.16 | ~$4.80 |
| Claude Sonnet | ~$0.38 | ~$11.40 |
| Gemini 2.0 Flash | ~$0.04 | ~$1.20 |

**You're currently using the lowest-cost option for daily use.** 🎯

---

## 🚀 Next Steps

1. **Verify it's working:** Send `/model` to the bot (should show current model)
2. **Test DeepSeek:** Send a message and confirm it's using DeepSeek 4
3. **Keep defaults:** DeepSeek is optimal for your use case
4. **Switch when needed:** Use `/model claude` for complex tasks requiring premium reasoning

---

## Config File

Current config at `/home/hermeswebui/.hermes/config.yaml`:
```yaml
model:
  default: deepseek-reasoner
  provider: deepseek
```

To change back to Claude Sonnet (not recommended for cost-first):
```yaml
model:
  default: claude-sonnet-4-5-20250929
  provider: anthropic
```

---

**Last Updated:** May 19, 2026  
**Strategy:** Cost-First (DeepSeek 4 default)  
**Status:** ✅ Optimized for your use case
