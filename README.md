# Karl Preisner

I’m a software engineer (M.S. Computer Science, GWU) with **8 years** of industry experience building machine learning systems, GPU-accelerated algorithms, and production distributed platforms across the full stack. As Sindri Labs’ first technical hire, I helped secure **$10M in venture funding** and built ZK proving infrastructure running across hundreds of GPU machines at 99.99% uptime, production LLM agents, and full-stack product features; the proving platform reached **$1M in annual recurring revenue**. Before Sindri, I was a **U.S. Government researcher**. In both roles, I worked directly with customers and senior leadership to turn their requirements into deployed systems.

My strengths are ML and AI agent design and optimization, algorithm design and benchmarking, CUDA/C++ performance tuning, and reliable APIs and SDKs.

## Portfolio

My portfolio site is at [karl.preisner.us](https://karl.preisner.us).

- **[MSR: Markovian Semantic Relatedness](https://github.com/KPreisner/markovian-semantic-relatedness):** Unsupervised query expansion and cross-language search. MSR runs a Markov-chain walk over a term co-occurrence graph to build a weighted concept that can rank untranslated foreign-language text for an English query, without machine translation. I designed MSR and led the project as a U.S. Government researcher (2019–2022); this is a from-scratch reimplementation.  
  ▶️ [Live demo](https://msr.preisner.us) · [Code](https://github.com/KPreisner/markovian-semantic-relatedness) · [Paper](https://msr.preisner.us/MarkovianSemanticRelatedness_april_25_2022.pdf)
- **[CHIP: Confounding Hash Iteration for Passwords](https://github.com/KPreisner/chip):** An iterated password hash that keeps hashing until it has seen a set number of collisions among the low bits of its digests, so the iteration count depends on the password and salt in a way you can't predict without running the whole chain.  
  ▶️ [Live demo](https://karl.preisner.us/chip/) · [Code](https://github.com/KPreisner/chip) · [Paper](https://github.com/KPreisner/chip/blob/main/docs/paper.md)
- **[Sagittal MSM](https://medium.com/@sindrilabs/sagittal-msm-a-streamlined-msm-implementation-a9dcc07da585):** A faster approach to [multi-scalar multiplication (MSM)](https://www.zprize.io/prizes/accelerating-msm-operations-on-gpu-fpga) of [elliptic-curve points](https://en.wikipedia.org/wiki/Elliptic_curve_point_multiplication), one of the most expensive steps in [zero-knowledge proving](https://en.wikipedia.org/wiki/Zero-knowledge_proof). I invented the mathematical approach, built Python operation models and a C++ reference, then directed and reviewed CPU/GPU implementations with colleagues and a Draper Labs contractor. It doubled processing throughput and outperformed the winning [2022 ZPrize](https://www.zprize.io/blog/announcing-zprize-results) GPU entries in internal benchmarks. Those results were a crucial part of the technical case behind Sindri's $5M seed round, led by [CoinFund](https://www.coinfund.io).  
  📄 [Article](https://medium.com/@sindrilabs/sagittal-msm-a-streamlined-msm-implementation-a9dcc07da585) · Code coming soon

## What I’ve worked on

### Sindri Labs: Founding Engineer, Lead Developer, Director of Engineering (2022–2026)

I joined as Sindri’s first technical hire and wrote core product code throughout, from GPU proving infrastructure to APIs, SDKs, and production LLM agents. I grew the engineering team to 7+ and led system design and code review. I worked directly with customers to translate high-level requirements into system designs and then built them, and I delivered the core product architecture, technical vision, and investor-ready benchmarks that helped secure $10M in venture funding.

- **AI agents:** Designed and built production agents for Deck, Sindri’s AI executive assistant, that routed user requests, searched project files, used integrations, and configured automations, and migrated its agent stack from direct OpenAI Responses API calls to the Agents SDK. I tuned agents from production traces, added automatic context trimming for long-running sessions, and benchmarked model upgrades against real-world requests before rollout. I also built Deck’s text extraction pipeline for dozens of file types, which produced more complete text than OpenAI's file ingestion in internal benchmarks.
- **Zero-knowledge proving:** Invented the mathematical approach behind [Sagittal MSM](https://medium.com/@sindrilabs/sagittal-msm-a-streamlined-msm-implementation-a9dcc07da585), which doubled throughput, beat the winning 2022 ZPrize GPU entries in internal benchmarks, and helped underpin Sindri’s $5M seed round. I designed and built much of the parallel proof execution system running across hundreds of GPU machines on GKE and CoreWeave, and led code review. It powered a general-purpose proving API that handled bursts of thousands of requests per minute at 99.99% uptime, reached $1M in ARR, and served customers including Zircuit and Zerion's ZERO Network. I also owned its [open-source Python SDK](https://github.com/Sindri-Labs/sindri-python).
- **Confidential AI:** Built an OpenAI-compatible API gateway for model inference in Intel TDX enclaves, and designed and implemented the encryption prototype for client-to-enclave requests and streamed responses.
- **Blockchain analytics:** Built Python and Django services for token and NFT event analysis, cryptocurrency price ingestion, and wallet segmentation.

### U.S. Government: Computer Systems Researcher (2019–2022)

- **Semantic search research:** Led a team of 10+ building [Markovian Semantic Relatedness (MSR)](https://github.com/KPreisner/markovian-semantic-relatedness), a cross-language retrieval system using unsupervised learning and graph analytics. It cut analyst search time by 50%.
- **Computer vision research:** Built a real-time system that used a high-speed camera and CUDA to recover sound from the vibrations of ordinary objects, turning days of post-processing into real-time output.

Most of my professional code is in private company repositories, so my contribution activity is more visible here than the source itself.

## Education

**The George Washington University**  
M.S. in Computer Science; B.S. in Computer Science with minors in Mathematics and Music.

**Fun fact:** I played trumpet in the Carolina Crown Drum and Bugle Corps from 2013 to 2016, including as lead trumpet, performing for 1/2 million people a year. In 2013 we won the World Championship ([watch the performance](https://www.youtube.com/watch?v=o8E8MJQgFog)) 🎺

## Technical skills

- **Languages:** Python, C/C++, CUDA, TypeScript/JavaScript, Java, SQL, Go, Rust, Bash, MATLAB
- **ML and AI:** PyTorch, TensorFlow, scikit-learn, Hugging Face Transformers, OpenCV, NumPy, SciPy, pandas, spaCy; OpenAI Responses API and Agents SDK, MCP, vector search and retrieval, agent evaluation, MLflow
- **GPU and performance:** CUDA, CuPy, cuBLAS, cuSPARSE, Thrust, NVIDIA Nsight, cuda-gdb, Valgrind, CMake
- **Sensors and embedded systems:** high-speed cameras, FLIR cameras, Ouster LIDAR, Arduino, Raspberry Pi, servo/stepper motor control, real-time signal and image processing
- **Backend and frontend:** Django (Ninja, DRF), FastAPI, Flask, Celery, asyncio, Pydantic; Next.js, React, Node.js
- **Cloud and infrastructure:** GCP/GKE, AWS (S3, ECS, EC2), CoreWeave, Kubernetes, Helm, Argo CD, Docker, GitHub Actions, NGINX, Traefik, NVIDIA Container Toolkit
- **Data, messaging, and observability:** PostgreSQL, SQLAlchemy, Alembic, PgBouncer, Redis, RabbitMQ, Kafka, NATS JetStream, Prometheus, Grafana, Loki, Sentry
- **ZK and cryptography:** Circom, Gnark, Noir, Halo2, Plonky2, SP1, RISC Zero, MSM/NTT, key exchange and authenticated encryption
- **Testing and tooling:** pytest, Vitest, Ruff, mypy, ESLint, uv, Poetry, Claude Code
