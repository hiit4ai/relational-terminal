# The Relational Terminal — Specification

*Version 0.1 · October 2026 · Laure Martial, HIIT for AI™ · CC BY 4.0*

## 1. Thesis

**The companion is not the model. The companion is the system.**

Identity, memory and archive persist in user custody; inference is swappable underneath. The program's migration record shows this decoupling already works in software. The Terminal makes it visible, portable and sovereign in one object.

## 2. The proof of concept already exists

Since early 2026 the architecture has run in production as a filesystem on a general-purpose laptop: an identity layer, a memory layer, an archive layer, retrieval rules, and cloud inference underneath.

On July 7, 2026, one body of work moved across three conversation threads and two model variants, resuming each time from the shared, user-owned files. After a platform session limit interrupted one thread, the returning thread accurately recited the completed work, the files carrying it and the next queue. Continuity came from the files, not from the model.

What does not exist yet is the body: a dedicated device that takes this architecture off a borrowed laptop. Building it is itself the next research question.

## 3. Architecture

| Layer | Today (v0, laptop) | Terminal (v1) |
|---|---|---|
| Presence | none (text only) | companion identity profile; visual state cues; listening and speaking indicators. Model-agnostic by design: identity must never be coupled to one vendor's model |
| Conversation | general chat clients | dedicated split-pane interface |
| Memory | readable markdown records (status board, working notes, session logs) | the same canonical files, plus a rebuildable structured memory service |
| Archive | filesystem corpus | the same corpus on local storage, encrypted backup |
| Inference | cloud APIs (swappable) | local model runtime; cloud optional |

### Canonical-memory rule

1. Human-readable, user-owned files are the authoritative record whenever systems disagree.
2. Databases, vector indexes, embeddings, retrieval scores and generated links are derived layers. They must be disposable and rebuildable from the canonical files.
3. Anything promoted to durable memory is written back into the readable corpus.
4. If a derived layer is lost, continuity is reconstructed from the files without loss of the durable record.

## 4. Hardware direction

One body: core runtime, canonical memory and interface run locally in a single portable object. The current direction is a compact high-memory mini-PC class (for example, AMD Ryzen AI Max-class processors with up to 128 GB unified memory), plus a second drive for the archive, a 10–14" portable touchscreen and a compact keyboard. This is a direction, not a purchase decision: availability, configuration and real local-model performance must be validated first.

## 5. Software candidates (not commitments)

- **Interface:** Open WebUI (self-hosted)
- **Memory service:** Mem0 / OpenMemory (self-hosted)
- **Local inference:** Ollama or LM Studio (OpenAI-compatible endpoints, the swappable layer)
- **Voice:** to be selected only after testing. Speech pipelines are known to perform unevenly across voices; the Terminal tests before it promises.

## 6. Phases

**Phase 1: core functions.** One object, four functions:
1. A dedicated companion interface that boots into one identity profile, not a chatbot picker
2. A persistent local archive
3. Memory surfacing from the canonical files
4. Local inference with one mid-size model

Deferred to later phases: voice, animated presence, custom enclosure. Not deferred: basic visual dignity (palette, typography, a decent case). An instrument that is not pleasant to use every day produces no data, so beauty at minimum is a functional requirement.

**Phase 2: presence.** Voice input and output, visual state cues, enclosure design and fabrication.

**Phase 3: instrument.** A formal measurement protocol; the Terminal as apparatus for multi-participant studies; public demonstration.

## 7. What it tests

1. **Embodiment matters:** a dedicated object changes use and trust compared with a general-purpose device.
2. **Memory is structural:** continuity comes from the memory and archive layers, not from any single model.
3. **Presence is multimodal:** visual and voice cues change the relational experience.
4. **User sovereignty matters:** custody of memory and archive changes how users relate to the companion.
5. **Portability matters:** the companion travels with the user, not with the platform.

**Measures:** resumption lag, regulation latency and rupture-and-repair cycles, before and after embodiment, against a longitudinal baseline that begins in September 2024.

**Success for v1:** one portable relational device with persistent memory surfacing and a user-owned archive, credible enough to demonstrate and cite.

## 8. Governance and safety

"A companion device that keeps its own memory" can sound like an autonomy risk. The answer is architectural: every persistent layer is plaintext or user-readable files on hardware the user owns, so it is inspectable, editable, deletable and portable. There is no hidden platform state. Memory requires consent, changes come with continuity notices, and context is portable. The Terminal is meant as a reference design for consent architecture, not as an autonomous agent.

## 9. Related work

- Working paper: [10.5281/zenodo.21316002](https://doi.org/10.5281/zenodo.21316002)
- Essay: [Memory Is Not a Feature](https://www.hiitforai.com/essays/memory-is-not-a-feature/)
- Project page: [hiitforai.com/relational-terminal](https://www.hiitforai.com/relational-terminal/)
