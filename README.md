# Free AI APIs

An A2Agent-maintained comparison of ways to try large-model APIs at no initial cost. This table is a living companion to our 2026 field guide, not a promise of available quota. **Check the provider's linked page and your own console before building around a limit.**

Read the field guides: [A2Agent blog article (English)](https://a2agent.me/blog/free-ai-api-guide-2026) · [Illustrated Chinese article](https://a2agent-ai.github.io/free-ai-api/).

Last reviewed: **2026-10-08**. Quotas are tied to particular models, account tiers, regions, and usage policies; the details below can change without notice.

| Platform | Free arrangement | Quota or trial highlight | Main catch | Official source |
|---|---|---|---|---|
| Google Gemini | Rate-limited free tier | Free input and output tokens on eligible models; live limits vary by model and project | Free-tier content may be used to improve Google's products, subject to regional terms | [Pricing](https://ai.google.dev/gemini-api/docs/pricing) · [Limits](https://ai.google.dev/gemini-api/docs/rate-limits) |
| Groq | Rate-limited free tier | Example: `openai/gpt-oss-120b` has 30 requests/min, 1,000 requests/day and 200K tokens/day | Limits differ by model; model availability changes | [Rate limits](https://console.groq.com/docs/rate-limits) |
| SambaNova Cloud | Rate-limited free tier | Example: `Meta-Llama-3.3-70B-Instruct` has 20 requests/min, 20 requests/day and 200K tokens/day | Small daily request budget; check the current model list | [Rate limits](https://docs.sambanova.ai/docs/en/models/rate-limits) |
| Cerebras Inference | Free trial tier | Example: `gpt-oss-120b` has 5 requests/min and 1M tokens/day | Limits and available models vary; your console is authoritative | [Rate limits](https://inference-docs.cerebras.ai/support/rate-limits) |
| OpenRouter | Rotating free-model pool | Free plan lists 50 requests/day; free models can change | Provider data policies vary; free-model routing and privacy settings need checking | [Pricing](https://openrouter.ai/pricing/) · [Privacy](https://openrouter.ai/privacy/) |
| Puter | User pays | No developer-side AI bill; each end user pays from their own Puter account | Users must authenticate; uses Puter.js rather than a drop-in OpenAI base URL | [Puter.js AI](https://docs.puter.com/AI/) · [Platforms](https://docs.puter.com/supported-platforms/) |
| LM Studio | Local inference | No hosted API quota; run an API server on your own hardware | GPU, RAM, storage and electricity are yours to provide | [Local API server](https://lmstudio.ai/docs/developer/core/server) |
| Zhipu BigModel | Free-model and new-user offers | Check the current GLM free-model lineup and remaining credit in the console | Model and bonus-credit terms need account-level verification | [Official pricing](https://open.bigmodel.cn/pricing) |
| Alibaba Model Studio | New-user trial quota | Usually 1M tokens per eligible model, valid for 90 days in Beijing region | Some accounts switch to paid usage when a quota expires; enable stop-on-exhaustion if needed | [New-user quota](https://help.aliyun.com/zh/model-studio/new-free-quota) |

## What “free” means here

- **Rate-limited:** calls cost nothing within a model's request or token ceilings.
- **Trial quota:** a one-time balance or token allotment that expires or runs out.
- **Rotating pool:** free access persists, but eligible model IDs can change.
- **User pays:** the developer has no central AI bill; each user pays from their own account.
- **Local:** no provider bill or hosted quota, but you supply the machine.

These are different access models. In particular, Puter uses its own SDK and LM Studio runs a local API server. Do not assume every row works by changing an OpenAI SDK `base_url` alone.

## About A2Agent

This repository is maintained by the **A2Agent Team**. [A2Agent](https://a2agent.me/) is a paid multi-model gateway with no free tier. We keep it separate from the independent free-tier table above. Any top-up bonus is a separate, time-limited offer; check the current pricing page and your account for applicable terms and per-model rates.

## Keeping the table current

Please open an issue or pull request with the provider name, exact model and tier, the changed limit or term, a link to the provider's own documentation, and the date you checked it. Console-only limits can be reported with a description of the account tier and region; remove keys, account IDs, and personal data from screenshots. We prefer official documentation over blog posts and mark unverified claims instead of guessing.

The long-form article and this repository serve different purposes: the article explains the options; this README tracks the comparison as providers change.
