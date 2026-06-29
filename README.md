# PA-Tool: Pretraining-Aligned Tool Schema Generation

Official repository for the **ACL 2026 (Main)** paper
**"Don't Adapt Small Language Models for Tools; Adapt Tool Schemas to the Models"**

Jonggeun Lee, Woojung Song, Jongwook Han, Haesung Pyun, Yohan Jo · Seoul National University

[📄 Paper (arXiv)](https://arxiv.org/abs/2510.07248) · [📚 ACL Anthology](https://aclanthology.org/2026.acl-long.948/) · [🌐 Project Page](https://holi-lab.github.io/PA-Tool/)

## Abstract

Small language models (SLMs) enable scalable tool-augmented multi-agent systems where multiple SLMs handle subtasks orchestrated by a powerful coordinator. However, they struggle with tool-use tasks, particularly in selecting appropriate tools and identifying correct parameters. A common failure mode is *schema misalignment*: models hallucinate plausible tool names that are absent from the provided tool schema, due to different naming conventions internalized during pretraining. Rather than training models to adapt to unfamiliar schemas, we propose adapting schemas to align with models' pretrained knowledge. We introduce **PA-Tool** (Pretraining-Aligned Tool Schema Generation), a training-free method that leverages *peakedness*, a signal used in contamination detection that indicates pretraining familiarity, to rename tool components. By generating multiple candidates and selecting the candidate with the highest peakedness, PA-Tool identifies pretraining-aligned naming patterns. Experiments on MetaTool and RoTBench show improvements of up to 17%, with schema misalignment errors reduced by 80%.

## Project page

This repository hosts the project page (`index.html` + `static/`), served via GitHub Pages. To preview locally:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Citation

```bibtex
@inproceedings{lee-etal-2026-dont,
    title = "Don{'}t Adapt Small Language Models for Tools; Adapt Tool Schemas to the Models",
    author = "Lee, Jonggeun and Song, Woojung and Han, Jongwook and Pyun, Haesung and Jo, Yohan",
    booktitle = "Proceedings of the 64th Annual Meeting of the {A}ssociation for {C}omputational {L}inguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2026",
    address = "San Diego, California, United States",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2026.acl-long.948/",
    pages = "20695--20719"
}
```

---

The project page was built using the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template).
