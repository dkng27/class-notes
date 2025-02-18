# Generative AI for Everyone

## Toolset

- Supervised learning
    - Biggest set
    - A → B
- Unsupervised learning
- Reinforcement learning
- ➡️ Generative AI is a different subset under AI (?)
    - Using supervised learning → next word prediction

## LLM as thought partner / general purpose tool

1. Find information
    - Hallucination: make stuff up
    - Don't use for authority info etc. → web search
2. Writing partner
    - Come up with ideas / names
    - Press release
    - Translation
        - Prompt engineering
3. Reading
    - Summarize
        - Emails
        - Call conversation
        - Reputation monitoring (reviews)
    - Proofreading
4. Chatting
    - Customer service
    - ➡️ bots support humans (human-in-the-loop)
        - catch bot errors
        - bot triage for humans (only hard questions)
    - IT service
    - Speicalized advice

- Deploying chatbots:
    - internal use only
    - avoid public mistakes
    - human-in-the-loop
    - ➡️ allow bot to talk directly after deemed safe

## Types of applications

- Web interface
    - Chatgpt brain storming
- Software automation / app (no UI)
    - email routing, document search

## LLM Cons

- Mental model: fresh grad analogy
- No memory of previous prompts
- No specific domain knowledge
- Knowledge cutoff
- Hallucinations
- Token limit
- Problem with tabular data
    - ✅ unstructured data: text, audio, images etc.
- Bias from training data
- Do not input sensitive data

## Tips for Prompting

- Details and context
- Guide the model (manual chain of thought)
    - Steps
- Iterate and clarify
    1. idea
    2. prompt
    3. response

## Image Generation (Diffusion)

- Iteratively denoise image (~steps)
- Pair with text caption alongside noisy image

## Retrieval Augmented Generation (RAG)

- Give context to chatbot with company documents
    - Search relevant text in company docs
    - Text incorporated into prompt
    - Link to original source doc
→ Summarize pdf, websites
⇒ LLM as reasoning engine: process instead of store information

## Fine-tuning

- Shift LLM response style with smaller training set
- Carry out task hard to define in single prompt
- Specific Domain knowledge
- Distillation (smaller edge model)

## Pretraining

- General purpose LLMs: expensive
- Mostly choose pretrained model and fine tune to what you want
- Only use if you have $ or have highly specialized domain
    - eg bloomberg financial model

## Choosing a model

### Model Size

- 1B param
    - Match pattern and general knowledge
- 10B
    - Follow basic instructions
- 100B+
    - Complex reasoning

### Closed vs Open Source

- Full control vs ease of use
- Run on device
- Vendor lock-in
- Data privacy

## Instruction Tuning && RLHF

- Train to follow instructions
    - Fine tuning with good question-answer pairs
        - Without it, LLM might keep generating questions
- Reinforcement learning from human feedback
    - Helpful, Honest, Harmless
    - Respond rated by humans to give rewards
    - Tune LLM to generate high score answers

## Tool Use

- Fine tune system message and user response
    - Trigger other software components
    - ➡️ Good practice: user confirmation
- Agent for tool use: eg calculator
    - Assisted by other software triggered by keywords in LLM response
        - e.g., `CALC()`
    - Generate steps for action and call other software components
