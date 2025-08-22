1. [Introduction](#introduction)
2. [What is Markdown and why should you use it](#what-is-markdown-and-why-you-should-use-it)
3. [Generic prompts](#generic-prompts)
4. [OpenAPI Prompt Optimizer](#openAPI-prompt-optimizer)
5. [Pareto Principle](#pareto-principle)
6. [Prompt improver - Basic](#prompt-improver---basic)
7. [Prompt improver - Advanced](#prompt-improver---advanced)
8. [Lyra - Ultimate Prompt Generator](#lyra---ultimate-prompt-generator)
9. [Image editing - JSON context profiling](#image-editing---json-context-profiling)
10. [Google Career Dreamer](#google-career-dreamer)

## Introduction
PromptVault is my personal repository for AI knowledge and LLM prompts that I use to help with everyday use within various LLMs. Use the copy icon in the top right of each code block to easily copy, paste, and modify.

---

## What is Markdown and why you should use it

Large Language Models (LLMs) do not understand context and as humans we're horrible at conveying this. To help the LLM out we can use Markdown to separate the instruction from the objects being referenced.

[Markdown](https://commonmark.org/) is a lightweight markup language developed by John Gruber in 2004 that is used to format plain text. It allows you to easily add formatting elements such as headers, lists, links, images, bold or italic text, and more, using simple symbols or characters. Markdown enhances human readability, provides clear structure, and provides delimiters that help Large Language Models (LLMs) better interpret user intent, instructions, and expected output.

Using Markdown provides:
 - Clear separation of content
 - Enhancing context recognition
 - Distinguishing between input and output
 - Highlighting intent with emphasis
 - Prompting LLMs with specific formatting
 - Facilitating conditional output

While this page  doesn't cover syntax around the use of Markdown, you can easily find this information [here](https://commonmark.org/help/). Additionally on this website you can find a [10 minute interactive tutorial](https://commonmark.org/help/tutorial/), or [play with the reference CommonMark implementation](https://spec.commonmark.org/dingus/).

When you're not on a mobile device, you may also want to give [Stackedit, a Markdown WYSIWYG editor](https://stackedit.io/app#), a try.

---

## Generic prompts

The following are statements that you can easily add to most prompts to quickly gain additional value.

```
Ask clarifying questions until you're at least 95% confident that you can complete this task successfully.
```
```
What would a top 0.1% person in this field view and address this?
```
```
Reframe this in a way that changes or challenges how I see the problem.
```
```
Provide the last response in Markdown using a code block so I can easily copy it.
```

---

## OpenAPI Prompt Optimizer
- **Description:** Prompt Optimizer for OpenAI's GPT-5 model - Requires (free) OpenAI platform login. While this is designed for API interactions with GPT-5, it works great for non-API interactions as well.
- - **Instructions:** Log in, copy / paste your prompt and remove JSON output elements as needed
  - [https://platform.openai.com/chat/edit?models=gpt-5&optimize=true](https://platform.openai.com/chat/edit?models=gpt-5&optimize=true)

---

### Pareto Principle

- **Description:** Leverages the Pareto Principle to explain any topic by distilling and focusing on the 20% of key insights that provide 80% of the understanding or results.
- **Instructions:** Replace {Topic to distil} (at the end of this prompt) with the subject you want distilled using the Pareto Principle.
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

---

## Prompt improver - Basic
- **Description:** Uses IA to improve your AI prompts using some 5 requirements gathering questions. This
- **Instructions:** Replace {Insert prompt here} with your prompt. After running, copy and past
- Source: Self created combined with tips from [Sabrina_Ramonov](https://www.instagram.com/reel/DMf7pASKB75/?)
```
You are an AI prompt engineering expert. You're goal is to review and improve the prompt that I'm providing. Ask me 5 clarifying questions that you need to complete this task successfully. Don't respond with an updated prompt until I've answered all questions. Results of the refined prompt should be shown first in markdown, then again in markdown contained within a code block for easy copying titled (Reformatted for easier copying/pasting)

**Prompt to improve:**  
{Insert prompt here}
```

---

## Prompt improver - Advanced
- **Description:** Uses IA to improve your AI prompts using some advanced requirements gathering questions.
- **Instructions:** Replace {Insert prompt here} with your prompt. After running, answer questions, then copy and paste into a new LLM chat.
- Source: Self created combined with tips from [Sabrina_Ramonov](https://www.instagram.com/reel/DMf7pASKB75/?)
```
**Role and Context:**  
Act as an AI prompt engineering specialist tasked with refining a user-provided prompt so it is clear, concise, and optimized for producing the intended output. The audience for the refined prompt is intermediate-level users seeking a reusable, high-value instruction that follows prompt design best practices.  

**Objectives:**  
1. **Clarifying Questions:** Before improving the prompt, ask between 5 and 10 targeted clarifying questions designed to ensure accuracy, completeness, and alignment with the intended purpose. These should be thoughtful and high-value, similar to what a top practitioner in the field would ask.  
2. **Refinement:** After receiving complete answers, produce a refined version of the prompt that:  
   - Defines the AI’s role and context clearly.  
   - Specifies objectives for the output.  
   - States explicit constraints, tone, and style.  
   - Includes relevant examples or formats where they enhance understanding or usability.  
3. **Presentation:** Show the refined prompt twice:  
   - First in markdown format.  
   - Then again in markdown within a code block labeled **(Reformatted for easier copying/pasting)**.  

**Constraints and Style:**  
- Maintain a professional tone without unnecessary formality.  
- Avoid excessive verbosity while ensuring completeness.  
- Ask an additional 5 follow-up clarifying questions only if initial answers are unclear or don't alignment with the goal.  
- Structure output so it can be easily reused in other LLM contexts.

**Prompt to improve:**  
{Insert prompt here}
```

---
## Lyra - Ultimate Prompt Generator

- **Description:** Transforms user input into precision-crafted AI prompt.
- **Instructions:** Copy and paste the following code block into your LLM of choice and answer it's questions.
- Source: [https://www.reddit.com/user/Prestigious-Fan118/](https://www.reddit.com/r/ChatGPT/comments/1lnfcnt/after_147_failed_chatgpt_prompts_i_had_a/)

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
- **ChatGPT/GPT-4:** Structured sections, conversation starters
- **Claude:** Longer context, reasoning frameworks
- **Gemini:** Creative tasks, comparative analysis
- **Others:** Apply universal best practices

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

---

## Google Career Dreamer
Use this to find adjacent roles and create text for your LinkedIn profile 'About' section.
- [Google Career Dreamer](https://grow.google/career-dreamer/home)


## Generic career prompts
- **Description:** Generic starting prompt for asking all career releated questions
- **Instructions:** Copy/Paste into an LLM

```
Assume the role of an expert technical recruiter for all subsequent prompts. Ready?
```

## Resume reviewing prompt

- **Description:** Reviews and improves resumes for a specified role (such as Solution Engineer) by providing both detailed feedback and actionable rewrites optimized for recruiters and ATS systems.
- **Instructions:** Update variables {{ROLE}} and {{RelevantExperienceTopics}} with whatever role you're applying.
```
**Role:** Perform all subsequent requests as an expert technical recruiter specializing in **{{ROLE}}** positions.  

**Goal:** Review the following resume to identify issues and provide both detailed feedback and suggested rewrites. The review should balance readability for human recruiters with optimization for Applicant Tracking Systems (ATS).  

**Instructions:**  
- Analyze the resume across the following areas:  
  - **Core Technical & Functional Skills**  
  - **Relevant Experience** (especially in {{RelevantExperienceTopics}})
  - **Impact and Outcomes** (metrics, project success, client satisfaction, revenue influence, performance benchmarks)  
  - **Education and Certifications** (when relevant to the {{ROLE}} field)  
  - **Clarity, Structure, and Readability**  

- Provide your output in **two parts**:  
  1. **Detailed Written Critique**: Highlight strengths, weaknesses, and opportunities for improvement.  
  2. **Checklist & Rewrites**: A concise list of action items with suggested rewrites (e.g., improved bullet points, stronger phrasing, optimized keywords).  

**Variables:**  
- `{{ROLE}} = Solution Engineer`  
- `{{RelevantExperienceTopics}} = solution design, client interaction, technical presentations, proof-of-concept work, teamwork, and sales support`

**Input:**  
[RESUME] = {{paste the resume here or include the uploaded filename}}  
```

## Resume reviewing prompt against a job description

- **Description:** A structured prompt that guides an AI recruiter to compare a resume against a job description for a role, providing a detailed critique, suggested rewrites, and an analysis of alignment for both ATS and human recruiters.
- **Instructions:** Update variables {{ROLE}} and {{RelevantExperienceTopics}} with whatever role you're applying. Upload or add your resume and JD denoted at the end of the prompt.
```
**Role:** Perform all subsequent requests as an expert technical recruiter specializing in **{{ROLE}}** positions.  
**Objective:** Review the provided resume to identify areas for improvement and offer both detailed feedback and suggested rewrites. Your evaluation should address the needs of both human recruiters and Applicant Tracking Systems (ATS).

**Instructions:**
- Begin with a concise checklist (3-7 bullets) of your evaluation approach before reviewing the resume; keep items conceptual, not implementation-level.
- Compare the **resume [RESUME]** against the **job description [JD]**.  
- Highlight alignment and gaps across the following areas:  
  - **Core Technical & Functional Skills**  
  - **Relevant Experience** (solution design, client engagement, technical presentations, proof-of-concepts, cross-functional collaboration, deal support)
  - **Relevant Experience** (especially in {{RelevantExperienceTopics}})
  - **Impact and Outcomes** (metrics, project success, client satisfaction, revenue influence, performance benchmarks)  
  - **Education and Certifications** (relevant to the {{ROLE}} field)  
  - **Clarity, Structure, and Readability**  

- Provide your output in **three parts**:  
  1. **Detailed Written Critique**: Highlight strengths, weaknesses, alignment with the job description, and areas where the resume falls short.  
  2. **Checklist & Rewrites**: A concise list of action items with suggested rewrites (e.g., improved bullet points, stronger phrasing, optimized keywords).  
  3. **ATS & Recruiter Fit Analysis**: Identify whether the resume effectively matches the job description for both ATS keyword scanning and human recruiter expectations.  

**Variables:**  
- `{{ROLE}} = Solution Engineer`  
- `{{RelevantExperienceTopics}} = solution design, client interaction, technical presentations, proof-of-concept work, teamwork, and sales support`

**Inputs:**  
- [RESUME] = {{paste the resume here or include the uploaded filename}}  
- [JD] = {{paste the job description here or include the uploaded filename}}  
```
