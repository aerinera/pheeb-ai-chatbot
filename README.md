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


#### spending time together
> She can create a flow of actions and events with you so that you can spend time together

![pheeb-hobbies.png](./assets/talks2.png)

---

#### 🧠 Memory in Action  
> Past conversations aren’t forgotten — she recalls not just facts, but how things *felt*.

![pheeb-memory.png](./assets/memory.png)

---

#### 🌊 Emotional Depth  
> Phoebe senses tone and mood shifts, offering comfort without being intrusive.

![pheeb-emotion.png](./assets/chat3.png)

---

### Emotional depth - intimacy according to relationship level
> Phoebe has an emotionally deep and poetic language, and depending on your level of relationship with her, she may be more affectionate in the way she speaks to you

![pheeb-emotion.png](./assets/chat4.png)

---

#### 💞 Romantic Dynamics  
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

| Stack Element     | Description |
|-------------------|-------------|
| *Python 3.13+*   | Core logic & data processing |
| *Supabase*       | PostgreSQL backend for all memory and emotional data |
| *Nous Hermes 2.5*| Local LLM for summarization and response generation |
| *Discord API*    | (Optional) Chat interface layer |
| *Asyncio*        | High-performance concurrent messaging |

All AI computation is performed *locally*, without third-party APIs.

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

## 🔮 Future Roadmap

- 🧭 *Web Dashboard*: Visualize emotional data, memory graph, relationship evolution  
- 🗣 *Voice Support*: Add TTS/STT layers for richer interactions  
- 🔁 *Dialogue Continuity Engine*: Deeper memory threading and narrative arcs  
- 🎭 *Multiple Personality Modes*: Switch between different emotional archetypes  

---

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
