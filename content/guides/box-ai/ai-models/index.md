---
rank: 1
related_guides:
  - box-ai/ai-tutorials/ask-questions
  - box-ai/ai-tutorials/generate-text
  - box-ai/ai-agents/get-agent-default-config
  - box-ai/ai-tutorials/default-agent-overrides
alias_paths:
  - guides/box-ai/supported-models
---

# Supported AI models

## Using models

You can use the supported AI models:

- get the [default AI agent configuration][agent],
- override the AI agent configuration used in [`POST 2.0/ai/ask`][ask], [`POST 2.0/ai/text_gen`][text-gen], [`POST 2.0/ai/extract`][extract], [`POST 2.0/ai/extract_structured`][extract-structured] endpoints.

When using the `model` parameter your API calls, use the **API Name** visible on each tile and model card.

For example, to get the AI agent configuration for a specific model, use the [model][ai-model] parameter and provide the `azure__openai__gpt_4o_mini` API name. Make sure you use **two underscores** after the provider name.

<Message type='notice'>
The list may change depending on the model availability.
Models offered in **Preview** mode have not been fully performance-tested at scale and are made available on an as-is basis. You may experience variability in model/output quality, availability, and accuracy.
</Message>

<TileGrid rows="2">
    <Tile type="gpt" title="azure__openai__gpt_4o_mini" href="/guides/box-ai/ai-models/azure-openai-gpt-4o-mini-model-card">
      A multimodal model designed to handle lightweight tasks.
      <div>
        <strong style="background-color: #e8e8e8">Default for Box AI for Box Hubs</strong>
        <strong style="background-color: #e8e8e8">Default for Box AI for Docs</strong>
        <strong style="background-color: #e8e8e8">Default for Box AI for Box Notes Q&A</strong>
        <strong style="background-color: #e1ffe7">Available</strong>
      </div>
    </Tile>
    <Tile type="gpt" title="azure__openai__gpt_4o_2024_05_13" href="/guides/box-ai/ai-models/azure-openai-gpt-4o-2024-05-13-model-card">
      A multimodal model, highly efficient in handling complex, multi-step tasks.
      <div>
        <strong style="background-color: #e8e8e8">Chat</strong>
        <strong style="background-color: #e1ffe7">Available</strong>
      </div>
    </Tile>
    <Tile type="gpt" title="azure__openai__text_embedding_ada_002" href="/guides/box-ai/ai-models/azure-text-embedding-ada-002-model-card">
      A most capable 2nd generation text embedding model. Skilled in
      text search, code search, and sentence similarity.
      <div>
        <strong style="background-color: #e8e8e8">Embeddings</strong>
        <strong style="background-color: #e1ffe7">Available</strong>
      </div>
    </Tile>
    <Tile type="gemini" title="google__gemini_2_0_flash_001" href="/guides/box-ai/ai-models/google-gemini-2-0-flash-001-model-card">
      Gemini multimodal model designed for optimal for high-volume, high-frequency tasks at scale.
      <div>
        <strong style="background-color: #e8e8e8">Chat</strong>
        <strong style="background-color: #e1ffe7">Available</strong>
      </div>
    </Tile>
    <Tile type="gemini" title="google__gemini_2_0_flash_lite_preview" href="/guides/box-ai/ai-models/google-gemini-2-0-flash-lite-preview-02-05">
      Gemini multimodal model designed to handle lightweight tasks.
      <div>
        <strong style="background-color: #e8e8e8">Chat</strong>
        <strong style="background-color: #e1ffe7">Available</strong>
      </div>
    </Tile>
    <Tile type="gemini" title="google__gemini_1_5_flash_001" href="/guides/box-ai/ai-models/google-gemini-1-5-flash-001-model-card">
      Gemini multimodal model, built for high volume tasks and latency-sensitive applications.
      <div>
        <strong style="background-color: #e8e8e8">Default for Box AI Extract</strong>
        <strong style="background-color: #e1ffe7">Available</strong>
      </div>
    </Tile>
    <Tile type="gemini" title="google__gemini_1_5_pro_001" href="/guides/box-ai/ai-models/google-gemini-1-5-pro-001-model-card">
        A foundation model that performs well at a variety of multimodal tasks.
      <div>
        <strong style="background-color: #e8e8e8">Chat</strong>
        <strong style="background-color: #e1ffe7">Available</strong>
      </div>
    </Tile>
    <Tile type="model" title="aws__claude_3_haiku" href="/guides/box-ai/ai-models/aws-claude-3-haiku-model-card">
      A model tailored for various language tasks, including creative writing and conversational AI.
      <div>
        <strong style="background-color: #e8e8e8">Chat</strong>
        <strong style="background-color: #fffbf3">Preview</strong>
      </div>
    </Tile>
    <Tile type="model" title="aws__claude_3_sonnet" href="/guides/box-ai/ai-models/aws-claude-3-sonnet-model-card">
       A model designed for advanced language tasks, focusing on comprehension and context handling.
      <div>
        <strong style="background-color: #e8e8e8">Chat</strong>
        <strong style="background-color: #fffbf3">Preview</strong>
      </div>
    </Tile>
     <Tile type="model" title="aws__claude_3_5_sonnet" href="/guides/box-ai/ai-models/aws-claude-3-5-sonnet-model-card">
      A model designed to enhance language understanding and generation tasks.
      <div>
        <strong style="background-color: #e8e8e8">Chat</strong>
        <strong style="background-color: #fffbf3">Preview</strong>
      </div>
    </Tile>
		<Tile type="model" title="aws__claude_3_7_sonnet" href="/guides/box-ai/ai-models/aws-claude-3-7-sonnet-model-card">
      A model designed to enhance language understanding and generation tasks.
      <div>
        <strong style="background-color: #e8e8e8">Chat</strong>
        <strong style="background-color: #fffbf3">Preview</strong>
      </div>
    </Tile>
     <Tile type="model" title="aws__titan_text_lite" href="/guides/box-ai/ai-models/aws-titan-text-lite-model-card">
      A model capable of advanced language processing, handling extensive contexts, making it suitable for complex tasks.
      <div>
        <strong style="background-color: #e8e8e8">Chat</strong>
        <strong style="background-color: #fffbf3">Preview</strong>
      </div>
    </Tile>
</TileGrid>

[ask]: e://post_ai_ask
[text-gen]: e://post_ai_text_gen
[extract]: e://post_ai_extract
[extract-structured]: e://post_ai_extract_structured
[agent]: e://get_ai_agent_default
[azure-ai-mini-4o-model]: https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/models?tabs=python-secure#gpt-4o-and-gpt-4-turbo
[vertex-ai-model]: https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#models
[vertex-ai-gemini-models]: https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#gemini-models
[vertex-text-models]: https://cloud.google.com/vertex-ai/generative-ai/docs/model-reference/text
[azure-ai-embeddings]: https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/models#embeddings
[ai-model]: e://get-ai-agent-default#param-model
[aws-claude]: https://aws.amazon.com/bedrock/claude/
[aws-titan]: https://aws.amazon.com/bedrock/titan/