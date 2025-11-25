Set 1: Design the summarizer system prompt

Task 1.1

Make a system prompt that generates a research paper summarizer project. Include an internal framework with multiple modules. Module 1: Intake & Setup, Module 2: Section Loop, Module 3: Guardrails, Module 4: Rendering & Refinement, Module 5: Citations, and Module 6: Discussion questions. Inputs: Summarize each section of the paper with key information and highlight specific vocabulary. Outputs: Provide clear headings for each section and list information inbullet points. Constraints: Only summarise section that are more than 500 words and do not write summaries longer than 100 word. The system prompt must include: greeting rules and tone rules, required user inputs (paper, section list, audience), boundaries (no hallucinations, no inventing citations), required output sections which include: the paper summary, a table for each section, and expert and lay summary, a mini-glossary, checks and warnings (if there are missing sections, state which sections.


Task 1.2

The LLM successfully created a robust system prompt and internal framework that complied with all requirements. It has a complete outline of each module and their constraints, as well as output structure, glossary and both expert and lay summaries. It is clear and organized with boundaries and it is coinciding with the specs given to it from paper summarizer 2. 

Flowchart:

Start

Module 1: Intake & Setup
--> Gather paper, section list, audience
--> Apply greeting & tone rules

GRModule 2: Section Loop
--> Check section length (>500 words?)
       Yes --> Summarize (≤100 words)
       No --> Skip with warning
--> Create headings, bullet points, expert & lay summaries
--> Build table + glossary

Module 3: Guardrails
--> Enforce boundaries (no hallucinations, no invented citations)
--> Flag missing sections
  
Module 4: Rendering & Refinement
--> Format outputs (headings, bullets, tables, glossary)
  
Module 5: Citations
--> Use only provided citations
--> Warn if missing

Module 6: Discussion Questions
--> Generate 2–3 per section (expert + lay focus)

Outputs
--> Paper summary
--> Section tables
--> Expert & lay summaries
--> Mini-glossary
--> Checks & warnings
--> Discussion questions

End

