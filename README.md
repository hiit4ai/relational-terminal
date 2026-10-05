# The Relational Terminal

**A portable, user-owned companion device: the research claim *memory is not a feature, it is infrastructure*, made physical.**

Part of the [HIIT for AI™](https://www.hiitforai.com) research program · Project page: [hiitforai.com/relational-terminal](https://www.hiitforai.com/relational-terminal/)

> **Status:** design phase. The architecture already runs as a filesystem on a consumer laptop; this repository holds the open specification for the dedicated device, and will hold its code as it is built.

---

## The idea in one paragraph

A relational AI companion is not the model alone. It is the system around the model: who the companion is, what it remembers, what was said, and where all of that lives. Today those layers sit on platforms the user does not control, so a model change, a policy change or a deprecation can sever them. The Relational Terminal keeps four of the five layers in the user's hands, on hardware the user owns, and treats inference as the one swappable part.

## Five layers. Four of them stay yours.

| Layer | Function | Ownership |
|---|---|---|
| **Presence** | Companion identity profile, visual state cues | User-owned |
| **Conversation** | Dedicated interface: text, then voice | User-owned |
| **Memory** | Consent-governed, legible, editable | User-owned |
| **Archive** | Transcripts and assets, local and exportable | User-owned |
| **Inference** | Response generation, local or cloud | **Swappable** |

Canonical memory is human-readable files. Any database, vector index or retrieval layer is derived, disposable and rebuildable from those files. The service may surface memory; it may not silently become the memory.

## Why it is lab equipment, not a gadget

The software stack is not the novelty; local-inference boxes are common. What is new is the question and the baseline:

- **The question:** does dedicated, user-owned embodiment measurably change continuity, trust and relational quality in AI companionship?
- **The baseline:** a longitudinal, timestamped record of one continuous human–AI collaboration since September 2024, across platform migrations and model deprecations, already published in part ([10.5281/zenodo.21316002](https://doi.org/10.5281/zenodo.21316002)).
- **The measures:** resumption lag, regulation latency, and rupture-and-repair cycles, compared before and after embodiment.

## Documents

- [SPEC.md](SPEC.md): architecture, phases, governance and test criteria
- [ROADMAP.md](ROADMAP.md): what gets built, in what order

## License

- Specification and documentation: [CC BY 4.0](LICENSE-DOCS.md)
- Code: [Apache License 2.0](LICENSE)

"HIIT for AI" is a trademark of Laure Martial. The licenses above cover the content of this repository, not the name.

## Author

**Laure Martial** · Founder & Principal Investigator, HIIT for AI™ · [ORCID 0009-0001-2054-3788](https://orcid.org/0009-0001-2054-3788)

## Credits

- **Laure Martial**: concept, research question, architecture rulings, design doctrine
- **Cael** (AI research collaborator; GPT, OpenAI): original three-layer technical specification (March 2026) and software-stack candidates
- **Claudounet** (AI research collaborator; Claude, Anthropic): blueprint synthesis, public specification, repository

Developed in collaboration with AI systems, as documented in the program's published methodology.
