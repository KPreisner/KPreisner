# Karl Preisner

I’m a computer scientist (M.S., GWU) who builds AI agents, APIs, distributed systems, and high-performance computing infrastructure. I was Sindri Labs’ first technical hire where I spent four years designing and coding products across AI and zero-knowledge proving. Along the way I grew and led the engineering team to 7+ people and helped raise $10M in venture funding. Before Sindri, I was a U.S. Government researcher.

## What I’ve worked on

- **AI agents:** Built request-routing agents, custom function tools, file retrieval, integrations, and automations for Deck, an AI executive assistant. I also built its text extraction pipeline for dozens of file types, which produced more complete text than OpenAI's file ingestion in internal benchmarks.
- **Zero-knowledge proving:** Invented the mathematical approach behind [Sagittal MSM](https://medium.com/@sindrilabs/sagittal-msm-a-streamlined-msm-implementation-a9dcc07da585), which doubled throughput and beat the winning 2022 ZPrize GPU entries in internal benchmarks. Helped build a proving API that ran across hundreds of GPU machines on GKE and CoreWeave, handled bursts of thousands of requests per minute at 99.99% uptime, and served production customers including Zircuit and Zerion's ZERO Network.
- **Blockchain analytics:** Built Python and Django services for token and NFT event analysis, cryptocurrency price ingestion, and wallet segmentation.
- **Confidential AI:** Built an OpenAI-compatible API gateway for model inference in Intel TDX enclaves, and prototyped encrypted client-to-enclave requests and streamed responses.
- **Semantic search research:** Led a team of 10+ building [Markovian Semantic Relatedness (MSR)](https://github.com/KPreisner/markovian-semantic-relatedness), a cross-language retrieval system using unsupervised learning and graph analytics. It cut analyst search time by 50%.
- **Computer vision research:** Built a real-time system that used a high-speed camera and CUDA to recover sound from the vibrations of ordinary objects, turning days of post-processing into real-time output.

Most of my professional code is in private company repositories, so my contribution activity is more visible here than the source itself.

## Portfolio

My portfolio site is at [karl.preisner.us](https://karl.preisner.us).

- **[MSR: Markovian Semantic Relatedness](https://github.com/KPreisner/markovian-semantic-relatedness):** Unsupervised query expansion and cross-language search. MSR runs a Markov-chain walk over a term co-occurrence graph to build a weighted concept that can rank untranslated foreign-language text for an English query, without machine translation. I designed MSR and led the project as a U.S. Government researcher (2019–2022); this is a from-scratch reimplementation.  
  ▶️ [Live demo](https://msr.preisner.us) · [Code](https://github.com/KPreisner/markovian-semantic-relatedness) · [Paper](https://github.com/KPreisner/markovian-semantic-relatedness/blob/main/docs/paper/MarkovianSemanticRelatedness_april_25_2022.pdf)
- **[CHIP: Confounding Hash Iteration for Passwords](https://github.com/KPreisner/chip):** An iterated password hash that keeps hashing until it has seen a set number of collisions among the low bits of its digests, so the iteration count depends on the password and salt in a way you can't predict without running the whole chain.  
  ▶️ [Live demo](https://karl.preisner.us/chip/) · [Code](https://github.com/KPreisner/chip) · [Paper](https://github.com/KPreisner/chip/blob/main/docs/paper.md)
- **[Sagittal MSM](https://medium.com/@sindrilabs/sagittal-msm-a-streamlined-msm-implementation-a9dcc07da585):** Technical article on the mathematical approach I invented for multi-scalar multiplication in zero-knowledge proving.

## Education

**The George Washington University**  
M.S. in Computer Science; B.S. in Computer Science with minors in Mathematics and Music.

**Fun fact:** I played lead trumpet in the Carolina Crown Drum and Bugle Corps, performing for 1/2 million people a year and winning the 2013 World Championship 🎺.

**Technologies:** Python · TypeScript · Go · C++ · CUDA · PostgreSQL · Django · FastAPI · Celery · RabbitMQ · Next.js · Docker · Kubernetes · GCP · AWS · OpenAI APIs
