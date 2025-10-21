## 🌍 What is StayCurious?

StayCurious is an open-source project that captures how people learn by *asking better questions*. A community-driven collection of **learning question paths** — sequences of prompts that guided people to understand topics deeply through conversation with AI.
> Instead of sharing *answers*, we share the *questions* that helped us learn.

We believe the future of learning is conversational — not about textbooks or lectures, but about structured curiosity and progressive inquiry.

---
## 💬 What’s in this repo?

This repository is a growing **library of learning question paths** — community-contributed collections of questions that helped people learn deeply through AI conversations.

---

### 🧠 1. Extract your learning questions

At the end of any deep ChatGPT or AI chat, paste this prompt to extract your **learning question path**:

~~~
I’ve been discussing a topic deeply in this chat. 
Please extract the **learning questions or prompts** from my conversation that could help someone else learn the same topic.

Here’s what you should do:
1. Identify the questions that contributed to learning or exploration.  
   - Ignore casual or personal talk.  
   - Focus on concept-building or reasoning questions.
2. Exclude anything that reveals personal or confidential information.
3. Organize the questions into **phases or themes**
4. Number questions within each phase.
~~~

---

### 📚 2. Courses organized by topic

All courses live inside the `/courses` directory, organized by broad subject areas:
~~~
courses/
┣ 📁 Health & Fitness/
┣ 📁 Technology/
┣ 📁 Finance/
┣ 📁 Science/
┣ 📁 Philosophy/
~~~

Each course is a Markdown file (`.md`) named after the topic and contains:
- A clear **title**  
- Phases of learning 
- Numbered **learning questions** in each phase  

Example:  
`courses/Health & Fitness/metabolism_fitness.md`

---

### 🤝 3. How to contribute

If you’ve created a new question path that others could learn from:

1. **Fork** this repository  
2. Add your `.md` file in the correct topic folder  
   - Example: `courses/Technology/ai_agents.md`
3. Submit a **pull request** with a short note like:  
> “Added ‘AI Agents Fundamentals’ course under Technology (4 phases, 28 questions).”

Once reviewed for clarity and privacy, your course will be merged into the library.
---
