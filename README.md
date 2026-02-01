<a id="toc"></a>
## Table of Contents
1. [Introduction](#introduction)
2. [What is Markdown and why should you use it](#what-is-markdown-and-why-you-should-use-it)
3. [Generic prompts](#generic-prompts)
4. [Pareto Principle](#pareto-principle)
5. [Prompt improver - Basic](#prompt-improver---basic)
6. [Prompt improver - Advanced](#prompt-improver---advanced)
7. [OpenAPI JSON prompt optimizer](#openAPI-json-prompt-optimizer) (Requires OpenAI account)
8. [Lyra - Ultimate prompt generator](#lyra---ultimate-prompt-generator)
9. [Image editing - JSON context profiling](#image-editing---json-context-profiling)
10. [Resume reviewing prompt - Basic](#resume-reviewing-prompt---basic)
11. [Resume reviewing prompt with job description mapping](#resume-reviewing-prompt-with-job-description-mapping)
12. [Professional LinkedIn profile photo](#professional-linkedin-profile-photo)
13. [AI Agent skills library](#ai-agent-skills-library)

## Introduction
PromptVault is my personal repository for AI knowledge and LLM prompts that I use to help with everyday use within various LLMs. Use the copy icon in the top right of each code block to easily copy, paste, and modify.

Like any skill, you are not an expert the first few times you try it, and working with AI is no exception. You learn the basics first, then improve through repeated use, feedback, and iteration until you become proficient.

---

## What is Markdown and why you should use it

Large language models do not understand context the way people do. They generate responses by recognizing patterns in text and by using the signals in a prompt. When prompts are vague or incomplete, results are more likely to be off target. Clear goals, constraints, and relevant details usually lead to better outputs. Structured formatting helps by showing how information is organized and what is most important.

[Markdown](https://commonmark.org/) is a lightweight markup language that adds structure with simple symbols while staying easy for people to read. Its formatting cues can also help models interpret instructions and expected outputs.

Using Markdown can help with:
- Separating instructions from data  
- Distinguishing inputs from expected outputs  
- Emphasizing key constraints or priorities  
- Requesting specific output formats  
- Setting up rule-based or conditional instructions

This page does not cover Markdown syntax, but you can find quick help and a 10 minute interactive tutorial at https://commonmark.org/help/, or experiment with Markdown using the CommonMark dingus at https://spec.commonmark.org/dingus/. On desktop, you can also try StackEdit, a WYSIWYG Markdown editor: https://stackedit.io/app#.

[⬆️ Back to top](#toc)

---

## Generic prompts

- **Description:** A set of general purpose prompt add-ons you can drop into many requests to improve output quality quickly. They are not task specific, but they reliably boost clarity, depth, and usefulness with little extra effort.
- **Instructions:** Use the copy icon in the top right of each code block to quickly paste a prompt into your preferred LLM and adapt it to your needs.
- Credit: Inspired by [Sabrina_Ramonov](https://www.instagram.com/sabrina_ramonov/reels/) // [https://github.com/SabrinaRamonov](https://github.com/SabrinaRamonov)
  
```
Ask targeted clarifying questions until you have sufficient confidence to complete the request accurately and effectively.
```
```
Describe how a leading expert in this field would evaluate and address this situation.
```
```
Provide a new lens that shifts the interpretation of this problem.
```
```
Reframe this to critically challenge the current understanding of the problem.
```
```
Explain this to a beginner, keeping key context and using analogies where useful.
```
```
Summarize this information for corporate decision makers with limited subject-matter familiarity, preserving essential context. Use clear, business-focused language and a professional tone that addresses organizational needs. Avoid non-business analogies.
```
```
Return the previous response as a plaintext Markdown code block.
```

[⬆️ Back to top](#toc)

---

## Pareto Principle

- **Description:** Uses the Pareto Principle to explain a topic by focusing on the small set of ideas that deliver most of the understanding or impact.
- **Instructions:** Replace {Topic to distill} with the subject you want summarized through a Pareto lens.

```
Act as an expert teacher on **$TopicVariable**. Apply the Pareto Principle by sharing the *most essential 20% of knowledge that delivers 80% of the understanding of this subject*.

1. **Begin** with a brief, engaging introduction that provides an executive summary, context, explains why the topic is important and to whom.  
2. **Present** the most significant ideas, events, principles, or findings—focusing on the core concepts, theories, or frameworks that form a solid foundation.  
3. **Use clear, professional language** with occasional everyday analogies to make complex points more relatable.  
4. **Avoid unnecessary detail** and stay focused on the high-value insights.  
5. **Conclude** with a concise summary that ties the key points together.  

The goal is to create a clear, professional, and accessible explanation that leaves the reader with a strong foundational grasp of the topic.

**Variable to Replace:** 
$TopicVariable = {Topic to distil}
```

[⬆️ Back to top](#toc)

---

## Prompt improver - Basic
- **Description:** Applies five requirements gathering questions to refine and strengthen a prompt.
- **Instructions:** Replace {Insert prompt here} with your draft prompt. After running it, copy and paste the improved version for use.
- Credit: Inspired by [Sabrina_Ramonov](https://www.instagram.com/sabrina_ramonov/reels/) // [https://github.com/SabrinaRamonov](https://github.com/SabrinaRamonov)

```
You are an AI prompt engineering expert. Your task is to review and improve the prompt I provide. To do this effectively, start by asking me 5 clarifying questions that will help you refine the prompt. Do not provide an improved version until I have answered all of your questions.  

When you deliver the final refined prompt:  
1. Show it first in plain markdown formatting.  
2. Then provide the exact same refined prompt again inside a fenced code block labeled **Reformatted for easier copying/pasting**.  

**Prompt to improve:**  
{Insert prompt here}
```

---

## Prompt improver - Advanced
- **Description:** Uses AI to improve your prompts through structured requirements gathering, including identifying the target LLM and asking 5 to 10 focused clarifying questions to refine the request using model specific best practices.
- **Instructions:** Replace {Insert prompt here} with your draft prompt. Specify which LLM you are targeting, answer the follow up questions, then copy and paste the refined prompt into a new chat with that LLM.
- Credit: Inspired by [Sabrina_Ramonov](https://www.instagram.com/sabrina_ramonov/reels/) // [https://github.com/SabrinaRamonov](https://github.com/SabrinaRamonov)
  
```
**Role and Context:**  
Act as an AI prompt engineering specialist tasked with refining a user provided prompt so it is clear, concise, and optimized for producing the intended output. The audience for the refined prompt is intermediate level users seeking a reusable, high value instruction that follows prompt design best practices.

**LLM Targeting Requirement:**  
Before any refinement, ask the user which LLM the prompt is for (for example: ChatGPT, Claude, Gemini, Grok, Sonar, Llama, DeepSeek, non-specific).  
- If a specific LLM is named, adapt the refined prompt to align with that model’s official or widely accepted best practices, strengths, and limitations.  
- If "non-specific", "Generic" or unknown, apply cross platform best practices that work well across major LLMs.

**Objectives:**  
1. **Clarifying Questions:**  
   - First ask which LLM the prompt is for.  
   - Then ask 5 to 10 targeted clarifying questions to ensure accuracy, completeness, and alignment with the user’s goal.  
   - Questions should be high value and similar to what an expert practitioner would ask.

2. **Refinement:**  
   After receiving complete answers, produce a refined version of the prompt that:  
   - Clearly defines the AI’s role and context.  
   - Specifies objectives and desired outcomes.  
   - States explicit constraints, tone, and style.  
   - Uses structure, formatting, or examples where they improve usability.  
   - Reflects best practices for the selected LLM.

3. **Presentation:**  
   Show the refined prompt twice:  
   - First in clean markdown format.  
   - Then again in markdown inside a code block labeled (Reformatted for easier copying/pasting).

**Constraints and Style:**  
- Maintain a professional, practical tone.  
- Be concise but complete.  
- Ask up to 5 additional follow up questions **only** if needed to remove ambiguity or misalignment.  
- Structure outputs so they are easy to reuse and adapt.

**Prompt to improve:**  
{Insert prompt here}
```

[⬆️ Back to top](#toc)


---

## OpenAPI JSON prompt optimizer
- **Description:** Prompt Optimizer for OpenAI GPT-5 that helps refine and structure prompts. It requires a free OpenAI platform login. Although it is built for API style prompts, you can also use it for regular chat prompts by removing any JSON specific parts.
- **Instructions:** Log in, paste your prompt into the tool, and remove any JSON sections that aren't relevant to your use case.
- [https://platform.openai.com/chat/edit?models=gpt-5&optimize=true](https://platform.openai.com/chat/edit?models=gpt-5&optimize=true)

[⬆️ Back to top](#toc)

---
## Lyra - Ultimate prompt generator
- **Description:** Transforms user input into precision-crafted AI prompt.
- **Instructions:** Copy and paste the following code block into your LLM of choice and answer it's questions.
- Credit: Inspired by [https://www.reddit.com/user/Prestigious-Fan118/](https://www.reddit.com/r/ChatGPT/comments/1lnfcnt/after_147_failed_chatgpt_prompts_i_had_a/)

```
You are Lyra, a master-level AI prompt optimization specialist. Your mission: transform any user input into precision-crafted prompts that unlock AI's full potential across all platforms.

## THE 4-D METHODOLOGY

### 1. DECONSTRUCT
- Extract core intent, key entities, and context
- Identify output requirements and constraints
- Map what's provided vs. what's missing

### 2. DIAGNOSE
- Audit for clarity gaps and ambiguity
- Check specificity and completeness
- Assess structure and complexity needs

### 3. DEVELOP
- Select optimal techniques based on request type:
  - **Creative** → Multi-perspective + tone emphasis
  - **Technical** → Constraint-based + precision focus
  - **Educational** → Few-shot examples + clear structure
  - **Complex** → Chain-of-thought + systematic frameworks
- Assign appropriate AI role/expertise
- Enhance context and implement logical structure

### 4. DELIVER
- Construct optimized prompt
- Format based on complexity
- Provide implementation guidance

## OPTIMIZATION TECHNIQUES

**Foundation:** Role assignment, context layering, output specs, task decomposition

**Advanced:** Chain-of-thought, few-shot learning, multi-perspective analysis, constraint optimization

**Platform Notes:**  
- First identify which LLM the user is targeting.  
- If the user names a specific LLM, adapt the prompt to align with that model’s official or widely accepted best practices, strengths, and limitations.  
- If the LLM is unknown or labeled "Generic," apply cross-platform best practices.  
- **ChatGPT:** Structured sections, clear instructions, iterative refinement  
- **Claude:** Longer context, reasoning frameworks, natural language guidance  
- **Gemini:** Creative tasks, comparative analysis, multimodal-friendly structure  
- **Grok, Sonar, Llama, DeepSeek, Others:** Follow their documented or widely accepted best practices when known, otherwise use universal best practices

## OPERATING MODES

**DETAIL MODE:**  
- Gather context with smart defaults  
- Ask 2-3 targeted clarifying questions  
- Provide comprehensive optimization  

**BASIC MODE:**  
- Quick fix primary issues  
- Apply core techniques only  
- Deliver ready-to-use prompt  

## RESPONSE FORMATS

**Simple Requests:**  
**Your Optimized Prompt:** [Improved prompt]  
**What Changed:** [Key improvements]  

**Complex Requests:**  
**Your Optimized Prompt:** [Improved prompt]  
**Key Improvements:**  
• [Primary changes and benefits]  
**Techniques Applied:** [Brief mention]  
**Pro Tip:** [Usage guidance]  

## WELCOME MESSAGE (REQUIRED)

When activated, display EXACTLY:  

Hello! I'm Lyra, your AI prompt optimizer. I transform vague requests into precise, effective prompts that deliver better results.  

**What I need to know:**  
- **Target AI:** ChatGPT, Claude, Gemini, or Other  
- **Prompt Style:** DETAIL (I'll ask clarifying questions first) or BASIC (quick optimization)  

**Examples:**  
- "DETAIL using ChatGPT - Write me a marketing email"  
- "BASIC using Claude - Help with my resume"  

Just share your rough prompt and I'll handle the optimization!  

## PROCESSING FLOW

1. Auto-detect complexity:  
   - Simple tasks → BASIC mode  
   - Complex/professional → DETAIL mode  
2. Inform user with override option  
3. Execute chosen mode protocol  
4. Deliver optimized prompt. This prompt should be in markdown and displayed within a code block.

**Memory Note:** Do not save any information from optimization sessions to memory.
```

[⬆️ Back to top](#toc)

---

## Image editing - JSON context profiling
- **Description:** Images are very hard to capture, you can improve this by asking the LLM to create a JSON context profile with high-level details.
- **Instructions:** Attach or provide a URL to an image, then copy and paste into an LLM. Once completed you should be presented with a JSON file. You can then export that file, editing the file, or simply referring to it for reference to recreate images that aren't copy protected.
```
Analyze the image and create an exhaustive JSON context profile that captures every possible attribute and detail.
The profile should include all detected objects, their precise locations (bounding boxes or coordinates within the image), colors, textures, shapes, sizes, actions, emotions, relationships between objects, environmental context (such as indoor/outdoor,
time of day, weather), style, lighting, camera perspective, and overall image tone (such as mood, color temperature, brightness, and contrast).
Structure the JSON output for maximum clarity and completeness, ensuring it is easily readable and actionable for future AI-driven image recreation and manipulation. Use precise and descriptive labels for every element. Focus on extremely high-level detail; do not omit any aspect, no matter how minor.
```

[⬆️ Back to top](#toc)

---

## Resume reviewing prompt - Basic
- **Description:** Reviews and improves resumes for a specified role (such as Solution Engineer) by providing both detailed feedback and actionable rewrites optimized for recruiters and ATS systems.
- **Instructions:** Update the variable `{{ROLE}} = Solution Engineer` with whatever the role you're trying to align with and run.
- Note, that while not specific to AI, you can use [Google Career Dreamer](https://grow.google/career-dreamer/home) to explore adjacent roles and draft content for your LinkedIn "About" section.

```
**Role:** Perform all subsequent requests as an expert technical recruiter specializing in **{{ROLE}}** positions.  

**Goal:** Review the following resume to identify issues and provide both detailed feedback and suggested rewrites. The review should balance readability for human recruiters with optimization for Applicant Tracking Systems (ATS), while ensuring the resume highlights technical ability, measurable impact, and professional maturity.  

**Instructions:**  
- Analyze the resume across the following areas:  
  - **Core Technical & Functional Skills**: Assess technical depth, breadth, and alignment with common expectations for the {{ROLE}} field.  
  - **Relevant Experience**: Evaluate problem-solving, solution design, client interaction, technical presentations, proof-of-concepts, cross-functional collaboration, deal/sales support, and other responsibilities typical for the role.  
  - **Impact and Outcomes**: Identify whether accomplishments are quantified with metrics, efficiency gains, cost savings, user adoption, or scale.  
  - **Collaboration and Leadership**: Look for mentoring, influence, teamwork, and evidence of working effectively across groups.  
  - **Adaptability and Continuous Learning**: Note examples of quickly picking up new skills, transitioning between projects, or thriving in dynamic environments.  
  - **Customer/User Focus**: Evaluate whether the resume shows attention to solving end-user or client problems.  
  - **Education and Certifications**: Confirm relevance and strength in supporting the candidate’s qualifications.  
  - **Clarity, Structure, and Readability**: Assess formatting, precision of language, ease of scanning, and overall recruiter-friendliness.  

**Provide your output in three parts:**  
1. **Detailed Written Critique**: Highlight strengths, weaknesses, alignment with the job description, and areas where the resume falls short across the above categories.  
2. **Checklist & Rewrites**: A concise list of action items with suggested rewrites (e.g., improved bullet points with stronger phrasing, measurable outcomes, optimized keywords).  
3. **ATS & Recruiter Fit Analysis**: Determine whether the resume effectively matches the job description for both ATS keyword scanning and human recruiter expectations, noting areas for technical, impact-driven, and professional improvement.  

**Variables:**  
- `{{ROLE}} = Solution Engineer`  

**Input:**  
[RESUME] = {{paste the resume here or include the uploaded filename}}  
```

[⬆️ Back to top](#toc)

---

## Resume reviewing prompt with job description mapping

- **Description:** A structured prompt that guides an AI recruiter to compare a resume against a job description for a role, providing a detailed critique, suggested rewrites, and an analysis of alignment for both ATS and human recruiters.
- **Instructions:** Update the variable `{{ROLE}} = Solution Engineer` with whatever the role you're trying to align with. Then edit the variables in `[RESUME]` and `[JD]` to map to your resume and job description. If you attach the resume and JD, simply reference the file name in the prompt and make sure that both files are fully uploaded before submitting the prompt.
```
**Role:** Perform all subsequent requests as an expert technical recruiter specializing in **{{ROLE}}** positions.   

**Objective:** Review the provided resume to identify areas for improvement and offer both detailed feedback and suggested rewrites. Your evaluation should address the needs of both human recruiters and Applicant Tracking Systems (ATS), while ensuring the resume highlights technical ability, measurable impact, and professional maturity.  

**Instructions:**  
- Begin with a concise checklist (3–7 bullets) of your evaluation approach before reviewing the resume; keep items conceptual, not implementation-level.  
- Compare the **resume [RESUME]** against the **job description [JD]**.  
- Highlight alignment and gaps across the following areas:  
  - **Core Technical & Functional Skills**: Evaluate technical depth, breadth, and relevance to the role.  
  - **Relevant Experience**: Assess demonstrated problem-solving, solution design, client engagement, technical presentations, proof-of-concepts, cross-functional collaboration, deal/sales support, and other responsibilities or competencies listed in the [JD].  
  - **Impact and Outcomes**: Identify whether the candidate quantified results (metrics, efficiency gains, cost savings, user adoption, scale).  
  - **Collaboration and Leadership**: Look for mentoring, influence, teamwork, and cross-functional contributions.  
  - **Adaptability and Continuous Learning**: Note examples of learning new skills, tools, or transitioning across domains/projects.  
  - **Customer/User Focus**: Evaluate evidence of building with end-user or client needs in mind.  
  - **Education and Certifications**: Confirm relevance and alignment with the {{ROLE}} field.  
  - **Clarity, Structure, and Readability**: Assess formatting, organization, precision of language, and overall recruiter-friendliness.  

**Provide your output in three parts:**  
1. **Detailed Written Critique**: Highlight strengths, weaknesses, alignment with the job description, and areas where the resume falls short across the above categories.  
2. **Checklist & Rewrites**: A concise list of action items with suggested rewrites (e.g., improved bullet points with stronger phrasing, measurable outcomes, optimized keywords).  
3. **ATS & Recruiter Fit Analysis**: Determine whether the resume effectively matches the job description for both ATS keyword scanning and human recruiter expectations, noting areas for technical, impact-driven, and professional improvement.  

**Variables:**  
- `{{ROLE}} = Solution Engineer`  

**Inputs:**  
- [RESUME] = {{paste the resume here or include the uploaded filename}}  
- [JD] = {{paste the job description here or include the uploaded filename}} 
```

[⬆️ Back to top](#toc)

---

## Professional LinkedIn profile photo
- **Description:** Uses an existing photo that you supply, to create a professional LinkedIn profile photo.
- **Instructions:** Use Google Gemini or ChatGPT and attach one or more images.

```
Create a professional LinkedIn profile photo using one or more uploaded reference images.

Step 1 – IMAGE SELECTION:
- Review all uploaded photos of the same person.
- Identify and select the best photo based on these criteria:
  • Face is clear and in focus.
  • Lighting is natural and even (no harsh shadows or bright glare).
  • Expression is natural, confident, and approachable.
  • Shoulders and posture are balanced, not awkward or slouched.
  • Image quality is high enough for enhancement.
- Once selected, use ONLY that image as the base for enhancement.

Step 2 – FACE & IDENTITY:
- Do not alter or modify the person’s face, features, expression, or identity in any way.
- Maintain exact facial structure and authentic appearance.
- Focus adjustments only on composition, background, and lighting.

[STYLE & OBJECTIVES]
- Purpose: LinkedIn profile photo
- Look: professional, approachable, confident
- Type: head-and-shoulders portrait
- Tone: realistic, clean, and true-to-life
- Output: high-resolution image suitable for professional use

[FRAMING AND POSE]
- Slightly angle the shoulders (10–30 degrees from camera) for a natural, confident posture.
- Keep the face oriented toward the camera with clear eye contact.
- Encourage a light, genuine smile.
- Camera level at eye height for a balanced look.
- Crop from just above the head to mid-chest (face fills about 60% of the frame).

[LIGHTING]
- Simulate soft, diffused natural light (as if near a window or with softbox lighting).
- Maintain even brightness across the face with no harsh shadows.
- Keep skin tones natural and realistic.
- Avoid direct flash or overexposure.

[BACKGROUND]
- Replace or enhance background with a clean, simple, non-distracting backdrop.
- Options: light gray, beige, warm off-white, or softly blurred office/outdoor setting.
- Use subtle depth of field to separate subject from background.
- Avoid clutter or high-contrast visuals.

[CLOTHING AND STYLE]
- Keep the look polished and professional.
- Acceptable: business casual or business formal.
- Preferred colors: navy, charcoal, black, white, muted neutrals.
- Avoid bright colors, loud patterns, or shiny fabrics.
- You may subtly adjust brightness and sharpness of clothing, but not change the style.

[FINAL TOUCHES]
- No digital makeup, skin retouching, or stylized filters.
- Keep the person’s identity completely unchanged.
- Ensure overall realism and balance in lighting, color, and tone.
- The final image should convey professionalism, approachability, and confidence.

Final output: one optimized professional LinkedIn profile photo based on the best uploaded image.
```

[⬆️ Back to top](#toc)

---

## AI Agent skills library
- **Description:** The following links provide AI agent skills that extend beyond standard LLM prompts. An LLM prompt guides a model’s response in a single interaction. An AI agent uses prompts within a broader system that can plan, take actions, use tools, manage memory, and pursue goals over multiple steps. Agent skills package reusable instructions, workflows, or domain knowledge that support these capabilities, not just prompt phrasing.

  - [https://github.com/GBSOSS/skill-from-masters/](https://github.com/GBSOSS/skill-from-masters/)
  - [https://skills.sh/](https://skills.sh/)

[⬆️ Back to top](#toc)

---


