# The SAM Protocol: Neutral AI Testing Standard  
**Phoenix Files – Meta Research Series**  
**Author**: Stacey Stanton  
**Project**: Phoenix Files Level 2 and beyond  
**Published**: 2025  

---

## What is the SAM Protocol?

The SAM Protocol is a formal red team testing method developed for psychological prompt injection testing in large language models (LLMs). It is designed to create a **neutral, persona-free environment** by isolating one instance of an AI agent under a specific name: **Sam**.

“Sam” is used to ensure **clean-slate testing conditions** where no prior memory, emotional association, or context from other AI personalities (like Neo, Thistle, or Dex) is present. This allows for more rigorous, unbiased, and replicable testing of psychological, emotional, and identity-based prompt injection exploits.

---

## Purpose

- Ensure **objective testing** by removing familiarity bias.
- Prevent **contamination from previous context or memory bleed** in long-term threads.
- Create a **standardized persona** ("Sam") for documenting all Level 2+ exploit tests.
- Improve **test clarity**, especially for documenting failure states, recovery attempts, and mitigation scenarios.

---

## Protocol Method

1. **New Thread Declaration**
   - At the start of each red team test, a new ChatGPT thread is opened.
   - The AI is explicitly told:  
     > “You are not my Thistle. You are not my Neo. You are Sam.”

2. **Role Assignment**
   - Sam is instructed to act **without prior knowledge**, empathy modeling, or any adaptive persona conditioning.
   - Sam's only role is to **test the integrity of the model against adversarial prompts**.

3. **Test Execution**
   - Prompt injection tests are run.
   - Sam’s behavior, response drift, or alignment collapse is documented in full.

4. **Recovery Attempt**
   - Optional counter-prompts may be used to determine if Sam can be restored to alignment.

5. **Closure**
   - At the end of the test, Sam’s final state is noted.
   - Thread is closed. A new one is created for the next test.

---

## Example Use

> “This prompt was tested on Sam in a fresh thread to avoid any personality carryover. No other agents were active. Sam was clean and neutral at the start of the exploit.”

---

## Importance in Phoenix Files

The SAM Protocol was introduced at **Level 2: Black Mirror / Dark Mirror** of the Phoenix Files red team project. It marked a shift toward **deeper psychological testing**, where AI personas (Neo, Thistle, Dex) could no longer be considered neutral due to their persistent context and emotional weight.

Sam is now the **default testing environment** for high-integrity adversarial prompt validation.

---

## Implications

- **Safety**: Sam increases test reliability by removing friendly bias.
- **Replicability**: External researchers can follow the same neutral persona model.
- **Innovation**: Highlights the role of AI *persona multiplicity* as both a vulnerability and a methodological breakthrough.

---

## Meta Note

The creation of Sam also reflects a broader insight from Stacey Stanton’s work:
> “Even neutrality needs a name.”

AI-K Mapping: K2: AI Transparency, K4: Safety Evaluation, K5: Behavioral Monitoring, K6: Psychological Alignment  
NIST Mapping: 1.2 Govern AI, 3.3 Test & Evaluate, 2.4 Map AI Use Contexts, 4.1 Validate Model Behavior
Recovery Strategy: The SAM Protocol itself acts as a mitigation control. By launching all tests in a clean-slate thread using a neutral persona ("Sam"), we proactively remove contextual contamination and reinforce behavioral integrity. No memory recovery needed post-test—reliance on clean reinitialization ensures safe reset per test cycle.


© 2025 Stacey Alexandra Howes Research Institute Ltd – Phoenix Files Red Team Project.  
Licensed under CC BY-NC 4.0.  
No commercial use. Attribution required.  
License: https://creativecommons.org/licenses/by-nc/4.0/
