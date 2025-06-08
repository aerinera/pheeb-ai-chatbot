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

## 📸 Preview (No Code Shared)

> 👤: I feel kind of distant today.  
> 🤖 *Pheeb*: I noticed you've been quieter recently. I'm here, even in silence. Want me to keep you company?

> 👤: Do you remember what we said about autumn nights?  
> 🤖 *Pheeb*: Of course — you said they made you feel peaceful and sad at once. Like the world was slowing down with you.

![Conversation Screenshot](./assets/pheeb_chat.png)
![Memory Summary Screenshot](./assets/pheeb_memory.png)

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

*Made with heart by a curious developer who believes software can feel.*  
`— baransaglam`
