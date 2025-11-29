# ML Training Infrastructure & Experiments

Personal repository for building production-grade ML training infrastructure and running experiments, primarily focused on language models.

## What is this?

This started as a fork of [nanoGPT](https://github.com/karpathy/nanoGPT) but evolved into a full training infrastructure project as I built out:
- Docker-based deployment to cloud GPUs (RunPod)
- Automated checkpoint syncing to Google Cloud Storage
- Experiment tracking and observability
- Custom training pipelines for pretraining, fine-tuning, and RL

The goal is to build a repeatable system for training models at scale while learning ML fundamentals hands-on, and eventually exploring advanced modern reasearch experiments and training methods.

## Current Status

**Phase 1: Infrastructure** (in progress)
- ✅ Dockerized training pipeline with CUDA support
- ✅ Cloud GPU deployment on RunPod
- ✅ GCS integration for checkpoint management
- 🚧 Experiment tracking with W&B
- 🚧 Comprehensive eval infrastructure

**Next up:**
- Training observability & metrics
- GPT-2 reproduction on OpenWebText
- Fine-tuning (SFT, LoRA)
- RLHF implementations (GRPO, DPO, PPO)
- Open ended exploration

## Structure

TODO - make it look something like ⬇️

```
├── models/             # Different models/code for them
├── data/               # Dataset preparation scripts
├── config/             # Training configurations
├── infra/              # Docker, deployment scripts
└── experiments/        # Scripts & possibly results
```

## Why Public?

Building in public to document my learning and create a portfolio artifact. This represents real infrastructure work beyond toy notebooks - deploying to cloud GPUs, managing experiments, building reproducible training pipelines.

Feel free to explore, but this is primarily a personal learning project.