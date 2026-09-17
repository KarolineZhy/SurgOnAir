# SurgOnAir: Hierarchy-Aware Real-Time Surgical Video Commentary

[![arXiv](https://img.shields.io/badge/arXiv-2605.21132-b31b1b.svg)](https://arxiv.org/abs/2605.21132)

**Jingyi He, Yue Zhou, Long Bai, Kun Yuan, Nassir Navab, Yuan Bi**

> 🚧 **Code and the SurgOnAir-11k dataset are coming soon.** Star / watch this repo to get notified.

## Demo

https://github.com/user-attachments/assets/c29f0261-31f4-4917-9a71-19fa32f6fc73

## Abstract

Understanding surgical workflow in real time is fundamental for intelligent surgical embodiment, where AI systems continuously perceive and respond as surgery proceeds. In the operating room, critical decisions depend on subtle, moment-to-moment changes, such as fine instrument movements and evolving tissue states, where even slight perceptual delays can limit assistance or compromise safety. Yet existing methods remain offline or operate at coarse temporal scales, generating descriptions only after processing clips, preventing immediate reaction.

We address this by proposing **SurgOnAir**, a streaming vision-language model that processes frames sequentially without future access and progressively generates narration tokens as visual input arrives. SurgOnAir achieves fine-grained frame-to-token generation, enabling instant responsiveness to evolving surgical dynamics. Built upon our curated hierarchical dataset **SurgOnAir-11k** spanning action-, step-, and phase-level supervision, the model is trained to produce multi-level textual responses that reflect the inherent hierarchy of surgical procedures. Furthermore, special transition tokens are generated to explicitly mark state changes, allowing SurgOnAir to capture and signal key workflow transitions as they occur.

Experiments show that SurgOnAir enables real-time understanding through a single vision-language model that unifies streaming across multiple hierarchies of the surgical workflow, generating superior and hierarchy-aware narrations.

## Highlights

- **Streaming inference** — frames are processed sequentially with no access to future frames; narration tokens are emitted as video arrives.
- **Hierarchy-aware narration** — a single model produces action-, step-, and phase-level commentary.
- **Explicit transition tokens** — workflow state changes are signalled the moment they occur.
- **SurgOnAir-11k** — a curated hierarchical dataset with action / step / phase supervision.

## Release plan

- [ ] Inference code and model weights
- [ ] Training code
- [ ] SurgOnAir-11k dataset

## Citation

```bibtex
@article{he2026surgonair,
  title   = {SurgOnAir: Hierarchy-Aware Real-Time Surgical Video Commentary},
  author  = {He, Jingyi and Zhou, Yue and Bai, Long and Yuan, Kun and Navab, Nassir and Bi, Yuan},
  journal = {arXiv preprint arXiv:2605.21132},
  year    = {2026}
}
```
