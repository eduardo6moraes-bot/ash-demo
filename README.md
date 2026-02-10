# ASH — AI-Orchestrated Cinematic Visual System

**ASH** is an experimental system that demonstrates how generative AI can be used not just to produce isolated media, but to **orchestrate modular cinematic narratives** by combining multiple short AI-generated visual fragments into a coherent visual experience.

---

## 🧠 Problem

Generative video models often produce short clips (e.g., 8 seconds) that can be limiting for storytelling.  
Instead of treating this as a drawback, ASH treats multiple short clips as **narrative building blocks**, forming a composable and scalable visual experience.

---

## 🛠️ Solution Approach

The system uses prompts crafted for cinematic quality and consistency, leveraging Google Gemini via API to generate short video segments.  
These segments are then curated and arranged to form a composed visual sequence.

The workflow includes:
- Prompt generation with cinematic visual guidance
- Model calls to Gemini API for video creation
- Post-generation organization of video segments
- Embedding and presentation on a demonstration page

---

## 🧪 Technical Details

**Built With:**  
- Gemini API (Google AI) — prompt-driven generation  
- Veo Studio / AI Studio — generation environment  
- HTML & CSS — demo site presentation  
- GitHub Pages — hosting  
- YouTube — video demo

Example of prompt structure used in generation:

