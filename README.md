# Odon

I build agents that actually do things, and the scaffolding that keeps them honest.

Applied AI engineer in Luxembourg. Right now: a computer-use agent for macOS that runs
entirely on-device, and an LLM pipeline translating a live publication in production.

I work under a handle. The work below is not anonymous — read it.

---

### What I'm building

**[Coherence](https://github.com/IAMOdon/coherence-overview)** — A computer-use agent for macOS running
**entirely on-device**. Two 4-bit models on MLX, accessibility-tree perception with a vision
fallback when an app exposes nothing, plan → execute → verify → replan over a KV-cached
session. 78k lines of Swift, 1,261 unit tests, CI building Debug *and* Release.
*Source private — overview, numbers, and access on request.*

**[NeuralSpace](https://github.com/IAMOdon/NeuralSpace)** — A deployed science-media platform
(Next.js 16, Supabase, Vercel) with a schema-constrained LLM translation pipeline inside it:
id-set integrity checking so a dropped paragraph is an error instead of a silent half-article,
a round-robin key pool with cooldown, retryable/fatal classification, cron-drained queue.
[Live](https://neural-space-hftk.vercel.app)

**[Macabre](https://github.com/IAMOdon/Macabre)** — watchOS app counting the heartbeats you
have left, from HealthKit data and cardiology literature. The math lives in one shared layer
compiled into both the app and the widget, so they can never disagree.

**[SoberCast](https://github.com/IAMOdon/SoberCast)** — watchOS blood-alcohol estimation from a
pharmacokinetic model (Widmark, first-order absorption / zero-order elimination). The algorithm
is documented separately from the code, because the algorithm is the product.

---

### How I work

Heavily agent-assisted development, under hard constraints I write down and version in the
repository: hardware target, memory budget, no network calls on user content, no
per-application special cases. Nothing is accepted until it survives a real execution trace.
I'd rather show the method than pretend it isn't part of the work.

I find the security holes in my own software and write them down with the date. Two of them
are in the repositories above — including the one where my own privacy-first app was shipping
user audio to a remote server.

---

### Stack

Swift · TypeScript · Python · MLX · Next.js · Supabase · PostgreSQL

---

### Open to

Applied AI and agent engineering roles. Remote or relocation, both fine.

[LinkedIn](https://www.linkedin.com/in/armand-wegnez/) · [armand.wegnez@gmail.com](mailto:armand.wegnez@gmail.com)
