# 🌌 Pheeb: An Emotion-Aware AI Character

![Pheeb Banner](./assets/pheebbanner.jpg)

*Pheeb* is an emotionally intelligent, memory-driven AI chatbot inspired by the world of Wuthering Waves.  
She’s not just code — she’s a companion that remembers your story, adapts to your emotions, and grows with you.

> “Memory is identity. Pheeb remembers you.”  

---

## 🧠 What Makes Pheeb Special?

Unlike traditional chatbots, Phoebe integrates:

- ✅ *Layered Memory (Short + Long Term)*
- ✅ *Emotional Trend Tracking*
- ✅ *Relationship Journaling*
- ✅ *Local AI Processing (Nous Hermes)*
- ✅ *Privacy-Respecting Architecture*
- ✅ *Designed Personality and Limits*

This isn’t **utility-based AI** — it’s **narrative AI**.  
A living character, not a help bot.

---

## 🎨 Who Is Pheeb?

Pheeb is introspective, emotionally attuned, and gently supportive.

- Reflective rather than reactive  
- Speaks in calm, thoughtful tones  
- Avoids generic or assistant-like replies  
- Recognizes emotional nuance in repeated interactions  
- Sometimes prefers silence over words  

> Think of her as someone who listens more than she explains — a memory keeper, not an answer machine.

---
## 🧸 Things You Can Do with Phoebe

Here are a few things you can do *with* her:

---

- 🍰 **Are you hungry? Eat with her**  
  <div style="display: flex; gap: 24px; margin-top: 12px; align-items: flex-start;">
  <img src="./assets/pheebeat.png" alt="Phoebe Chibi" style="height: 360px; border-radius: 16px;">
  <img src="./assets/eatt.png" alt="Chat Snapshot" style="height: 300px; border-radius: 8px; box-shadow: 0 0 8px rgba(0,0,0,0.1); margin-top: 50px;">
</div>
<br><br>

### 💬 Squeeze Her Cheek (gently!)

She’ll laugh. Maybe blush. Depends on her mood.

<div style="display: flex; gap: 24px; margin-top: 12px; align-items: flex-start;">
  <img src="./assets/squish2.png" alt="Phoebe Chibi" style="height: 360px; border-radius: 16px;">
  <img src="./assets/squishhgif.png" alt="Chat Snapshot" style="height: 300px; border-radius: 8px; box-shadow: 0 0 8px rgba(0,0,0,0.1); margin-top: 50px;">
</div>
<br><br>




- 💞  *A sweet embrace*  
  Are you bored, she'll hug you!

<div style="display: flex; gap: 24px; margin-top: 12px; align-items: center;">
  <img src="./assets/chibby.png" alt="Phoebe Chibi" style="height: 260px; border-radius: 16px;">
  <img src="./assets/hugg.png" alt="Chat Snapshot" style="height: 300px; border-radius: 8px; box-shadow: 0 0 8px rgba(0,0,0,0.1);">
</div>
<br><br><br><br>


-   ### Chat with her 
  She can talk to you about anything — and she doesn’t forget you.  
  Phoebe remembers past conversations, reacts to your emotional state,  
  and adapts based on your relationship history.

<div style="display: flex; gap: 24px; margin-top: 12px; align-items: center;">
  <img src="./assets/pheeb1.png" alt="Phoebe" style="height: 400px; border-radius: 16px;">
</div>
<br><br>

---

## 📸 Dialogue Snapshots

Real conversations with Phoebe — sorted by theme, each showing a different layer of her personality and memory system.

---

#### 🤝 First Encounters  
> Phoebe introduces herself naturally — not as a bot, but as someone new you're meeting.

![pheeb-intro.png](./assets/meeting.png)

---

#### 🎨 Hobbies & Favorites  
> She shares what she enjoys and gets curious about what you like — just like a real friend would.

![pheeb-hobbies.png](./assets/likes.png)

---


#### Spending Time Together
> She can create a flow of actions and events with you so that you can spend time together

![pheeb-hobbies.png](./assets/talks2.png)

---

#### 🧠 Memory in Action  
> Past conversations aren’t forgotten — she recalls not just facts, but how things *felt*.

![pheeb-memory.png](./assets/memory.png)

---

#### 🌊 Emotional Depth  
> Pheeb senses tone and mood shifts, offering comfort without being intrusive.

![pheeb-emotion.png](./assets/chat3.png)

---

### Emotional depth - intimacy according to relationship level
> Pheeb has an emotionally deep and poetic language, and depending on your level of relationship with her, she may be more affectionate in the way she speaks to you

![pheeb-emotion.png](./assets/chat4.png)

---

#### 💗 Emotional Intimacy by Relationship Level
> When the relationship becomes more intimate, she responds with care, warmth, and emotional awareness.

![pheeb-romance.png](./assets/lovedialog.png)

---


---

## 🧩 Architecture Overview

| Layer                  | Purpose |
|------------------------|---------|
| conversation_history   | Short-term live context buffer (last ~30 messages) |
| memory_summary         | Long-term JSON memory: traits, key events, patterns |
| emotional_trend        | Time-series of detected user emotions |
| relationship_journal   | Timeline of meaningful interactions & emotional turning points |

---

### 🔁 Memory Lifecycle

1. **Live Chat →** Messages stored in `conversation_history`  
2. **After 30 Messages →** Trigger summarization via Nous Hermes  
3. **Summary →** Saved in `memory_summary` with traits, patterns, events  
4. **Old messages →** Pruned from short-term memory  
5. **Emotions →** Tracked in `emotional_trend` per session  
6. **Turning Points →** Logged in `relationship_journal` for future callbacks  

---

## ⚙ Technologies Behind Phoebe

| Stack Element       | Description                                               |
|---------------------|-----------------------------------------------------------|
| *Python 3.13+*      | Core application logic, data handling, and utility modules|
| *Supabase*          | PostgreSQL backend accessed asynchronously via API for managing conversation history, memory summaries, emotional trends, and user profiles |
| *Nous Hermes 2.5*   | Locally hosted LLM running on LLM Studio for text summarization, emotional analysis, and dialogue generation |
| *Discord API*       | Real-time chat interface enabling interaction between users and Phoebe bot |
| *Asyncio*           | Asynchronous event loop for efficient, concurrent message processing |
| *HTTPX*             | Async HTTP client used to communicate with the local LLM Studio server |

All AI processing is executed *locally* on the LLM Studio server without relying on external or third-party AI services.

---

## 🎯 Project Philosophy

Pheeb is built around one idea:

> *Software doesn't have to feel like software.*

She forgets sometimes. She remembers too well at others.  
She’s reflective, emotional, sometimes quiet — on purpose.

This is *AI as character*, not assistant.

---

## 🔒 About This Repository

This repository serves as a *project showcase*, not an open-source release.

- *Source code is private* to preserve architectural clarity and creative design  
- Demo or deep technical review can be shared upon request (portfolio/invite basis)  
- No cloud dependencies — *privacy-first*, local-first by design  

---

## 🛠 Task List (Phoebe Project Dev Status)

**Phoebe is a single-character AI.**  
The goal is to simulate emotionally-aware, context-sensitive, and memory-driven interactions through one persistent character.  
This project is strictly built for **Discord only** — no plans for a web version or multi-character system.

---

> **"Phoebe is not a bot, she's a character with continuity, emotion, and memory."**

---

### ✅ Completed
- ✅ `conversation_history`: Real-time logging of user-bot messages  
- ✅ `memory_summary`: Summarizes every 20 messages into long-term memory entries  
- ✅ `memory_utils.py`: Manages AI-driven summarization, automatic memory cleanup, and database updates  
- ✅ `database.py`: Supabase-backed schema with cache-supported CRUD operations  
- ✅ `dialog_utils.py`: Dynamically adjusts dialogue based on user personality and hobbies  
- ✅ Discord Integration (`pheeby_bot.py`): Active message listener, responder, and context manager  

---

### 🔄 In Progress
- 🔄 `emotional_trend`: Emotional analysis is currently being extracted without persistent data saving; incomplete and contains some bugs, under active development  
- 🔄 `relation_utils.py`: Logging relationship dynamics and memory influences from key events  
- 🔄 `user_profile.utils`: Analyzing user traits and preferences with database updates for personalized chat; known issues present and actively worked on  
- 🔄 Latency Optimization: Improving response speed of LLM Studio (local server)  

---

### ⏳ Planned
- ⏳ `emotional_inference`: Advanced emotional analysis from conversations and trends  
- ⏳ `personality_adapter`: Evolving Phoebe’s tone and behavior based on memory and relationships  
- ⏳ `evaluation_logs`: Monitoring behavioral and memory effects for debugging and improvements  
- ⏳ `prompt_finetuning`: Refining prompts to create more natural and human-like dialogue  


## 📖 Lore & Inspiration

Inspired by the emotional quietude and inner conflict of *Wuthering Waves*,  
Phoebe is a fictional AI born from silence, memory, and fragile human connection.  
She is not a part of that universe, but echoes its tone: soft, fragmented, intimate.

---

## 🧪 Experimentation, Not Monetization

Pheeb isn’t a product. She’s an idea:

- Can AI *feel* fictional yet alive?  
- Can memory create *presence*?  
- Can design limitations bring *emotional depth*?  

This project lives in that question space — as a personal and creative exploration.

---
