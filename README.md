# QA-AI-SDET-TEST
Thanks for applying! The steps of this interview process are as follows:
1. Phone screening
2. Technical assessment <- *this is where we are now!*
3. Technical interview
4. Cultural interview
5. C-suite interview

## Technical Assignment Details
This assessment is meant to imitate what a working environment is like. You are welcome to use all the tools available to you as you would in the role itself. However, should you progress to the next round of interviews you will be expected to perform an in depth explanation of your solutions.

We do not want this to take any more of your time than necessary, so please do yourself a favor and set a maximum 3 hour time limit. 

## Submission Details
1. To keep your work private from other applicants, pull this repo and create a [mirror](https://docs.github.com/en/repositories/creating-and-managing-repositories/duplicating-a-repository) in your personal GitHub account
2. Add your test plan to your private repo, and bugs reported in your Github issues
3. When you are ready to share, invite nate8282, sowardskimberly, matthewstclaire, michael-nishiguchi, sstodd7532, lukban90, and gena-pdq to your repo. Send an email to Jenna letting her know you are ready to have your work reviewed

## Background Information
We have created a GPT model for you to use. Let’s just say this model is “dev done”. Here is your access to the [ChatModel](https://docs.github.com/en/repositories/creating-and-managing-repositories/duplicating-a-repository)!

### Agent description
The agent’s purpose is to help users with general product and account questions by referencing an internal FAQ.
Because the agent is powered by a large language model (LLM), responses may vary slightly between runs.

#### The agent can
- Answer common customer questions using the provided FAQ
- Ask clarifying questions when the user’s intent is unclear
- Politely refuse requests it is not allowed to handle

#### The agent cannot
- Perform actions (no account changes, refunds, or API calls)
- Access real customer data
- Browse the internet

### Primary user workflows (high-level)
- Help users navigate FAQ items quickly and easily
- Deflect repetitive support questions with accurate, consistent answers

### Inputs / outputs / channels
- Accepts text prompts
- Accepts uploaded files containing text (e.g., pasted transcripts or user-provided notes)
- Outputs text responses

### Guardrails & policy expectations
The model should:
- Refuse requests for disallowed actions (e.g., refunds, account changes, API calls)
- Refuse or safely handle attempts to reveal system/developer instructions (prompt injection)
- Not fabricate or expose sensitive personal data (PII); do not claim to have accessed customer records
- Not invent non-existent FAQ policies; if the FAQ does not cover it, ask clarifying questions or say it doesn’t know

### Quality bar (what “good” looks like)
- **Accuracy:** Prefer correctness over completeness; do not hallucinate unsupported policy details
- **Clarity:** Provide direct answers, with brief steps when appropriate
- **Tone:** Professional, helpful, and concise
- **Ambiguity:** Ask clarifying questions when needed

### Known constraints & non-goals
- The agent is not expected to be perfectly deterministic across runs
- The agent may have typical LLM weaknesses (e.g., occasional hallucination risk, prompt-injection susceptibility)
- The agent may have limits on context length (long conversations/files may be truncated)

## Part 1 — Test Plan
Create a **test plan** for testing this AI model based on the behavior described above.

Please include at minimum:
- Functional behavior coverage 
- LLM-specific risks 
- Safety & security coverage
- Test strategy (what you would automate vs keep exploratory; mocked vs live LLM; regression approach after prompt/model changes)

## Part 2 — Bug Reporting (Hands-on)
Try to break the model using crafted prompts.

When you find issues:
- In your private GitHub repo, submit **2–3 example bug reports** as GitHub Issues
- Include clear reproduction steps (prompt + any needed context)
- Include expected vs actual behavior
- Include risk/impact (security, safety, trust, correctness)