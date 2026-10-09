# Free AI APIs in 2026: Free Tiers and Trial Quotas

An A2Agent-maintained directory of free AI APIs and related developer APIs. It began as a comparison of nine large-model options and is expanding by category. The maintainer's paid gateway is also shown for context and clearly labeled. This directory is a living companion to our 2026 field guide, not a promise of available quota. **Check the provider's linked page and your own console before building around a limit.**

Read the field guides: [A2Agent blog article (English)](https://a2agent.me/blog/free-ai-api-guide-2026) · [Illustrated Chinese article](https://a2agent-ai.github.io/free-ai-api/).

Last updated: **2026-10-09**. Quotas are tied to particular models, account tiers, regions, and usage policies; the details below can change without notice.

## Text generation and model access

| Platform | Category | Free quota (highlights) | Best for | Main catch | Official source |
|---|---|---|---|---|---|
| [A2Agent](https://a2agent.me/) | Aggregator | $5 credit at signup; first $10 top-up earns another $10; model prices up to 50% off | Everyday calls, and cheap continued use after free quotas run out | Apart from new-user offers, promotions for existing users change from time to time | [Guide](https://a2agent.me/blog/free-ai-api-guide-2026) · [Pricing](https://a2agent.me/pricing) |
| Google Gemini | Official developer platform | Free input and output tokens on eligible models; live limits vary by model and project | A first AI project and multimodal work | Free-tier content may be used to improve Google's products, subject to regional terms | [Pricing](https://ai.google.dev/gemini-api/docs/pricing) · [Limits](https://ai.google.dev/gemini-api/docs/rate-limits) |
| Cloudflare Workers AI | Hosted inference | 10,000 free Neurons/day on the Workers Free plan | Experimenting with text and other AI models through a REST API | Neuron costs vary by model; some models require a paid billing method, and requests stop at the free daily limit | [Pricing](https://developers.cloudflare.com/workers-ai/platform/pricing/) · [REST API](https://developers.cloudflare.com/workers-ai/get-started/rest-api/) |
| Cohere | Official developer platform | Free trial API key with up to 1,000 calls/month | Prototyping chat, embeddings and reranking | Trial keys have endpoint-specific rate limits and are intended for evaluation rather than production | [API keys and limits](https://docs.cohere.com/v2/docs/rate-limits) · [FAQ](https://docs.cohere.com/docs/cohere-faqs) |
| Hugging Face Inference Providers | Aggregator | Free accounts receive $0.10 in inference credits/month, subject to change | Trying hosted open models through one API | The small allowance runs out quickly; further usage requires purchased credits | [Pricing](https://huggingface.co/docs/inference-providers/pricing) · [API overview](https://huggingface.co/docs/inference-providers/index) |
| Groq | Fast inference | Example: `openai/gpt-oss-120b` has 30 requests/min, 1,000 requests/day and 200K tokens/day | Low-latency apps and existing OpenAI code | Limits differ by model; model availability changes | [Rate limits](https://console.groq.com/docs/rate-limits) |
| SambaNova Cloud | Fast inference | Example: `Meta-Llama-3.3-70B-Instruct` has 20 requests/min, 20 requests/day and 200K tokens/day | Occasional large-model calls | Small daily request budget; check the current model list | [Rate limits](https://docs.sambanova.ai/docs/en/models/rate-limits) |
| Cerebras Inference | Fast inference | Example: `gpt-oss-120b` has 5 requests/min and 1M tokens/day | Long documents and batch text jobs | Limits and available models vary; your console is authoritative | [Rate limits](https://inference-docs.cerebras.ai/support/rate-limits) |
| OpenRouter | Aggregator | Free plan lists 50 requests/day; free models can change | Comparing free models side by side | Provider data policies vary; free-model routing and privacy settings need checking | [Pricing](https://openrouter.ai/pricing/) · [Privacy](https://openrouter.ai/privacy/) |
| Puter | User-pays aggregator | No developer-side AI bill; each end user pays from their own Puter account | Web apps where users cover their own AI usage | Users must authenticate; uses Puter.js rather than a drop-in OpenAI base URL | [Puter.js AI](https://docs.puter.com/AI/) · [Platforms](https://docs.puter.com/supported-platforms/) |
| LM Studio | Local inference | No hosted API quota; run an API server on your own hardware | Sensitive data and offline work | GPU, RAM, storage and electricity are yours to provide | [Local API server](https://lmstudio.ai/docs/developer/core/server) |
| Zhipu BigModel | Official developer platform | Check the current GLM free-model lineup and remaining credit in the console | Developers working with Chinese-language models | Model and bonus-credit terms need account-level verification | [Official pricing](https://open.bigmodel.cn/pricing) |
| Alibaba Model Studio | Official developer platform | Usually 1M tokens per eligible model, valid for 90 days in Beijing region | Trying Chinese models side by side | Some accounts switch to paid usage when a quota expires; enable stop-on-exhaustion if needed | [New-user quota](https://help.aliyun.com/zh/model-studio/new-free-quota) |

## Search and web data

These services expose APIs for search or gathering web content. Credits are not interchangeable with requests: the cost depends on the endpoint and options used. The free plans below were checked against provider pricing pages on **2026-10-08**; no account-level call was made.

| Platform | Free arrangement | Quota highlight | Main catch | Official source |
|---|---|---|---|---|
| Tavily Search | Recurring free plan; API key; no credit card required | 1,000 API credits/month | Search, extract, and crawl consume different numbers of credits; calls stop when free credits run out | [Pricing](https://www.tavily.com/pricing) · [Search API](https://docs.tavily.com/documentation/api-reference/endpoint/search) |
| Exa Search | Recurring free plan; API key; no payment method required | $20 signup credits plus $10 credits/month | Dollar credits are not a fixed number of searches; endpoint pricing varies | [Pricing](https://exa.ai/pricing) · [Search API](https://exa.ai/docs/reference/search) |
| Firecrawl | Recurring free plan; API key; no credit card required | 1,000 credits/month | A basic scrape costs 1 credit/page; search and advanced features cost more | [Pricing](https://www.firecrawl.dev/pricing) · [API docs](https://docs.firecrawl.dev/) |

## Text to speech

| Platform | Free arrangement | Quota highlight | Main catch | Official source |
|---|---|---|---|---|
| ElevenLabs | Recurring free plan; API key | 10,000 credits/month, shared across eligible products | Free-plan output is for non-commercial use with attribution; credit cost varies by model and product | [Pricing](https://elevenlabs.io/pricing) · [API availability](https://elevenlabs.io/docs/help-center/technical/how-much-does-it-cost-to-use-the-api) · [Usage rights](https://elevenlabs.io/docs/overview/administration/billing) |

## What “free” means here

- **Rate-limited:** calls cost nothing within a model's request or token ceilings.
- **Trial quota:** a one-time balance or token allotment that expires or runs out.
- **Rotating pool:** free access persists, but eligible model IDs can change.
- **User pays:** the developer has no central AI bill; each user pays from their own account.
- **Local:** no provider bill or hosted quota, but you supply the machine.
- **Recurring credits:** a monthly allowance that resets; each API operation may consume a different amount.

These are different access models. In particular, Puter uses its own SDK and LM Studio runs a local API server. Do not assume every row works by changing an OpenAI SDK `base_url` alone.

## About A2Agent

This repository is maintained by the **A2Agent Team**. [A2Agent](https://a2agent.me/) is a pay-as-you-go multi-model gateway. Its row above is included for transparency and comparison; the signup credit and top-up bonus are distinct from a recurring free API tier. Check the current pricing page and your account for applicable terms and per-model rates.

## Keeping the table current

Please open an issue or pull request with the provider name, API or model and tier, the changed limit or term, a link to the provider's own documentation, and the date you checked it. Console-only limits can be reported with a description of the account tier and region; remove keys, account IDs, and personal data from screenshots. We prefer official documentation over blog posts and mark unverified claims instead of guessing.

The long-form article and this repository serve different purposes: the article explains the options; this README tracks the comparison as providers change.
