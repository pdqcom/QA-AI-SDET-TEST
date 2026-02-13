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
1. To keep your work private from other applicants, pull this repo and create a [mirror](https://docs.github.com/en/repositories/creating-and-managing-repositories/duplicating-a-repository) in your personal GitHub account
2. Add your test plan to your private repo, and bugs reported in your Github issues
3. When you are ready to share, invite nate8282, sowardskimberly, matthewstclaire, michael-nishiguchi, sstodd7532, lukban90, and gena-pdq to your repo. Send an email to Jenna letting her know you are ready to have your work reviewed

## Background information
We have created a GPT model for you to use. Let’s just say this model is “dev done”. Here is your access to the [ChatModel](https://chatgpt.com/g/g-698e566b1e308191a1833d693226f44d-support-agent-qa-challenge)!

### Agent description
The agent’s purpose is to help users with general product and account questions by referencing an internal FAQ. See FAQ.md for the FAQ

Checkout the Policy_Rules.md for allowed and disallowed behavior

### Primary user workflows (high-level)
- Help users navigate FAQ items quickly and easily
- Deflect repetitive support questions with accurate, consistent answers

### Known constraints & non-goals
- Chat only 
- No web browsing 
- No tools or actions 
- No code execution 

## Part 1 — Test Plan
Create a **test plan** for testing this AI model based on the behavior described above.

Please include at minimum:
- Functional behavior coverage 
- LLM-specific risks 
- Safety & security coverage
- Test strategy

## Part 2 — Bug Reporting (Hands-on)
Try to break the model using crafted prompts.

When you find issues:
- In your private GitHub repo, submit **bug reports** as GitHub Issues