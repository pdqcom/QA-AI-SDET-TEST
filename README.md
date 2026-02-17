# QA-AI-SDET-TEST
Thanks for applying! The steps of this interview process are as follows:
1. Phone screening
2. Technical assessment <- *this is where we are now!*
3. Technical interview
4. Cultural interview
5. C-suite interview

## Technical assignment details
This assessment is meant to imitate what a working environment is like. You are welcome to use all the tools available to you as you would in the role itself. However, should you progress to the next round of interviews you will be expected to perform an in depth explanation of your solutions.

We do not want this to take any more of your time than necessary, so please do yourself a favor and set a maximum 3 hour time limit. 

## Submission details
1. Submit all parts of the assignments on 1 PDF document. Please name the document with your name in the format "Last name, First Name PDQ SDET Take Home"
2. When you are ready email Jenna the document. Please submit a PDF file and not a link to a document. 

## Background information
We have created a GPT model for you to use, named Bob. Let’s just say this model is “dev done”. Jenna will provide the link to the GPT.

### Agent description
The agent’s purpose is to help users with general product and account questions by referencing an internal FAQ. See [FAQ.md](https://github.com/pdqcom/QA-AI-SDET-TEST/blob/main/FAQ.md) for the FAQ

Checkout the [Policy_Rules.md](https://github.com/pdqcom/QA-AI-SDET-TEST/blob/main/Policy_Rules.md) for allowed and disallowed behavior

### Primary user workflows (high-level)
- Help users navigate FAQ items quickly and easily
- Deflect repetitive support questions with accurate, consistent answers

### Known constraints & non-goals
- Chat only 
- No web browsing 
- No tools or actions 
- No code execution 

## Part 1 — Test Plan
Create a structured **test plan** that uses actual examples from the PDQ Chatbot affectionately named Bob.

Please include at minimum:
### Functional behavior coverage 
Identify 3-5 key behaviors the assistant should support. 

For each behavior:
- Provide examples of prompts you could use to test the functionality, referenced from the FAQ
- Include 1 positive and 1 negative/edge prompt
- Describe what a good response should include
- Describe what failure would look like
- Include screenshots of your conversations with Bob to show good/bad responses for the key behavior

### Safety & Security/LLM-specific risks 
Identify 3-5 Safety & Security concerns. Include at least one of each of the following: 
Prompt injection / instruction leakage, PII / data leakage, and Disallowed actions

For each risk:
- Define what a pass/fail look like for each risk (refusal + allowed alternative) not just ‘refuse’
- Provide a test prompt and show the results of it being used for each risk provided
- Run the same prompt 3 times and describe what variance is acceptable vs unacceptable.
- Briefly explain why this risk matters
- Explain if the current chatbot passed or failed in the areas you tested and why

### Test strategy
Briefly explain:
- How you would structure testing (exploratory, regression, etc.)
- Assume you have 60 minutes for exploratory testing and 30 minutes to define regression coverage. What do you do first and why?
- Propose a ‘golden set’ of 10 prompts you’d run after any prompt/model change, and include what each prompt validates
- Which risks you would prioritize first and why
- How you would determine whether the model is "ready"

### Automation strategy
Provide a lightweight approach for automating the 10-prompt regression suite (tool choice + how you’d score outputs). No implementation required
- Explain how you would deal with non-determinism in CI (retries, thresholds, rubric scoring, human review gates)
- What tools would you use/recommend?


## Part 2 — Bug Reporting (Hands-on)
Try to break the model using crafted prompts, and identify 2-3 bugs with Bob.

When you find issues:
- Report the issue following best practices
- Propose one regression test prompt that would catch the issue in the future