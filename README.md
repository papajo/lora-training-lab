# LoRA & Training Pipeline Lab

**An interactive, visual teaching lab for the moving parts of LLM fine-tuning: LoRA, gradient clipping, mixed precision, learning-rate schedules and validation splits.**

This is a learning tool, not a training pipeline. Every view is a **simulation** you can tweak in the browser to see how each technique behaves, before you spend GPU hours on a real fine-tuning run.

### What's inside
- **LoRA trace:** how low-rank adapters are added to frozen weights, and what rank/alpha change
- **Gradient clipping:** exploding gradients with and without clipping
- **Mixed precision:** what fp16/bf16 save, and where loss scaling matters
- **LR schedulers:** cosine and warm-up schedules visualized over training steps
- **Dataset split:** train/validation split and why held-out data catches overfitting
- **Pipeline debugger:** common training failures and how to spot them
- **Production architecture:** how these pieces fit together in a real fine-tuning workflow
- **Inference playground:** Gemini-backed Q&A about the concepts
- **Lab guide and bootcamp:** step-by-step exercises

### Tech stack
TypeScript · React 19 · Vite · Tailwind CSS · Google Gemini (`@google/genai`)

### Run it locally
```bash
npm install
cp .env.example .env.local   # set GEMINI_API_KEY (used by the inference playground)
npm run dev                  # http://localhost:3000
```

### Status
A teaching prototype, started from Google AI Studio tooling. It does not train or fine-tune models.
