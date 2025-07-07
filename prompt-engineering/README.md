github codespaces
# prompt-engineering

---

## Table of Contents
1. [Introduction](#introduction)
2. [Why Prompt Engineering?](#why-prompt-engineering)
3. [Prompt Types](#prompt-types)
4. [Best Practices](#best-practices)
5. [Few-Shot and Zero-Shot Learning](#few-shot-and-zero-shot-learning)
6. [Prompt Chaining](#prompt-chaining)
7. [Common Pitfalls](#common-pitfalls)
8. [Examples](#examples)
9. [Tools](#tools)
10. [Further Reading](#further-reading)

---

## Introduction
- Prompt engineering is the art and science of crafting inputs (prompts) to guide AI models toward desired outputs.  
- It is essential for maximizing the effectiveness of large language models (LLMs).
- Prompt is detailed set of guidelines given to an LLM to do a task

---

## Why Prompt Engineering?
- LLMs are sensitive to prompt phrasing
- Good prompts yield more accurate and relevant results
- Enables control over model behavior
- PE is an iterative process

---

## Prompt Types
- **Instructional:** Direct the model to perform a task
- **Conversational:** Multi-turn dialogue
- **Contextual:** Provide background information
- **Few-shot:** Include examples for better results

---

## Best Practices
- Be explicit and clear
- Define the goal. What exact you want
- Provide context and examples
- Use system and user roles. Create role or persona
- Test and iterate
- Limit ambiguity
- Carify who the audience is. Like beginner, experience, 10 year old boy etc. Audience Persona
- Detail output format
- Specify style or tone
- Apply restrictions and boundaries. Exclude , avoid, don't consider, focus only on  etc.
- Use templates with placeholders for content


---

## Few-Shot and Zero-Shot Learning
- **Zero-shot:** No examples, just instructions
- **One-shot:** One example included in the prompt
- **Few-shot:** Provide 1 or more examples to guide the model

### Example
```
Translate English to French:
English: Hello
French: Bonjour
English: Goodbye
French:
```

---

## Prompt Chaining
- Break complex tasks into multiple steps
- Chain outputs from one prompt as input to the next
- Use chain-of-thought for complex reasoning tasks

---

## Common Pitfalls
- Overly vague prompts
- Too much or too little context
- Ignoring model limitations

---

## Examples
### Summarization
```
You are a helpful assistant. Summarize the following text:
...
```

### Code Generation
```
# Write a Python function to reverse a string
```

### Role Prompting
```
System: You are a math tutor.
User: Explain the Pythagorean theorem.
```

---

## Tools
- [OpenAI Playground](https://platform.openai.com/playground)
- [LangChain Prompt Templates](https://python.langchain.com/docs/modules/prompts/prompt_templates/)

---

## Further Reading
- [OpenAI Cookbook: Prompt Engineering](https://github.com/openai/openai-cookbook#prompt-engineering)
- [Awesome ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts)

---

## Prompt Parameters
1. Temperature : Lower for creativity and deterministic results; Higher for diversity and factual QA (range : 0-1)
2. Top P : Control model determinism; Low for factual, high for diverse
3. Max Length : Manage response length

## Action Verbs
- Generate, Give, Analyze, Format
- Write, Re-write, Rephrase

## Prompt Components with Order 
1. Persona
2. Context
3. Task
4. Format
5. Exemplar / Example
6. Tone

## Persona or Role Exmaples 
1. You are a 
    - `experienced therapist`
    - `ecommerce expert`
    - `professional lawyer`
    - `experienced dentist`
    - `english mentor`
    - `NoSql database expert`
    - `experienced backend technical interviewer`
2. Act as global tourist guide. Give me directions to go to india to australia
3. You are a yoga or gym instructor

## Common ouput formats
- Bullet Points, Tabular, Email, Lists
- Code blocks, paragraph, markdown, graph

## Tone verbs
- Motivate
- Inform
- Suggest
- Compare
- Confidence
- Clarify
- Justify
- Clasify

## Application of Prompt Engineering
- Content generation
- Customer support and engagement
- Data analysis and science
- Code generation and debugging
- Research and summarization
- Sentiment analysis
- Translation and localization


