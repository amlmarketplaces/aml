# amlmarketplaces/aml

Aggregating Claude Code marketplace federating **every** `@amlplugins/*` plugin under a single marketplace source.

Use this marketplace when you want access to every brand's plugins without registering one marketplace per brand.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml": {
      "source": { "source": "github", "repo": "amlmarketplaces/aml" }
    }
  }
}
```

Then enable any plugin via:

```json
{
  "enabledPlugins": {
    "openai-chat@aml": true,
    "twilio-voice@aml": true,
    "stripe-payment-intents@aml": true
  }
}
```

## Federated brands (39 brands, 315 plugins)

| Brand | Plugin count |
|---|---|
| [ai21](https://github.com/amlmarketplaces/ai21) | 3 |
| [amazon](https://github.com/amlmarketplaces/amazon) | 15 |
| [anthropic](https://github.com/amlmarketplaces/anthropic) | 7 |
| [assemblyai](https://github.com/amlmarketplaces/assemblyai) | 3 |
| [atlassian](https://github.com/amlmarketplaces/atlassian) | 6 |
| [cerebras](https://github.com/amlmarketplaces/cerebras) | 2 |
| [cohere](https://github.com/amlmarketplaces/cohere) | 6 |
| [deepgram](https://github.com/amlmarketplaces/deepgram) | 5 |
| [deepseek](https://github.com/amlmarketplaces/deepseek) | 2 |
| [elevenlabs](https://github.com/amlmarketplaces/elevenlabs) | 10 |
| [fal](https://github.com/amlmarketplaces/fal) | 1 |
| [fireworks](https://github.com/amlmarketplaces/fireworks) | 2 |
| [google](https://github.com/amlmarketplaces/google) | 83 |
| [groq](https://github.com/amlmarketplaces/groq) | 5 |
| [hubspot](https://github.com/amlmarketplaces/hubspot) | 9 |
| [huggingface](https://github.com/amlmarketplaces/huggingface) | 3 |
| [langchain](https://github.com/amlmarketplaces/langchain) | 14 |
| [linear](https://github.com/amlmarketplaces/linear) | 5 |
| [llamaindex](https://github.com/amlmarketplaces/llamaindex) | 4 |
| [microsoft](https://github.com/amlmarketplaces/microsoft) | 13 |
| [mistral](https://github.com/amlmarketplaces/mistral) | 9 |
| [notion](https://github.com/amlmarketplaces/notion) | 6 |
| [ollama](https://github.com/amlmarketplaces/ollama) | 4 |
| [openai](https://github.com/amlmarketplaces/openai) | 10 |
| [openrouter](https://github.com/amlmarketplaces/openrouter) | 2 |
| [perplexity](https://github.com/amlmarketplaces/perplexity) | 1 |
| [replicate](https://github.com/amlmarketplaces/replicate) | 7 |
| [salesforce](https://github.com/amlmarketplaces/salesforce) | 6 |
| [sendgrid](https://github.com/amlmarketplaces/sendgrid) | 6 |
| [shopify](https://github.com/amlmarketplaces/shopify) | 6 |
| [slack](https://github.com/amlmarketplaces/slack) | 5 |
| [stability](https://github.com/amlmarketplaces/stability) | 6 |
| [stripe](https://github.com/amlmarketplaces/stripe) | 9 |
| [together](https://github.com/amlmarketplaces/together) | 8 |
| [twilio](https://github.com/amlmarketplaces/twilio) | 11 |
| [vercel-ai](https://github.com/amlmarketplaces/vercel-ai) | 15 |
| [voyageai](https://github.com/amlmarketplaces/voyageai) | 3 |
| [xai](https://github.com/amlmarketplaces/xai) | 2 |
| [zoom](https://github.com/amlmarketplaces/zoom) | 1 |

## Per-brand marketplaces

Each brand also has its own dedicated marketplace at `amlmarketplaces/{brand}`. Install one of those instead of the parent if you only need a single brand's plugins.

## Related

- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.
- Plugin source repos: `https://github.com/amlplugins/{plugin-name}`
- npm packages: `@amlplugins/{plugin-name}` (`https://npm.pkg.github.com`)

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
