# Evaluating Human–LLM Alignments on Visualization Preference

This repository houses the supplementary material for the submission  
**"Evaluating Human–LLM Alignments on Visualization Preference"** at  
**IEEE VIS 2026 (Short Papers Track)**.

## User Study

1. **User Annotation UI**  
   [Open Annotation Interface](https://darthrevan07.github.io/chart-evaluation-new/)

2. **Pre-study and Post-study Questionnaires**  
   - [Pre-study Questionnaire](https://forms.office.com/r/6SgGDC2mDS)  
   - [Post-study Questionnaire](https://forms.office.com/r/k4bPxvZZYZ)  
   *(PDF versions available in `userStudy` folder)*

## Evaluation Results

1. A qualitative overview of human and model preference distributions on a pair-wise basis has been shown in `Preference Votes_Final.xlsx`
2. Model rationale and annotator notes (if provided) are available in `annotations/notes_by_pair.json`
3. The actual chart image pairs (in proper naming convention) is available in the directory `study_pairs`.

## Acknowledgements & Data Source

Parts of the dataset used in this work are derived from the dataset released with the paper  
**“$C^2$: Scalable Auto-Feedback for LLM-based Chart Generation”** (Koh et al., 2025)  
and its accompanying repository.

We gratefully acknowledge the authors for making their data and resources publicly available.

If you use this repository, please also cite the original *C2* paper and dataset.

## Citation

### BibTeX

```bibtex
@c{2koh2025c2scalableautofeedbackllmbased,
  title={$C^2$: Scalable Auto-Feedback for LLM-based Chart Generation},
  author={Woosung Koh and Jang Han Yoon and MinHyung Lee and Youngjin Song and Jaegwan Cho and Jaehyun Kang and Taehyeon Kim and Se-Young Yun and Youngjae Yu and Bongshin Lee},
  year={2025},
  eprint={2410.18652},
  archivePrefix={arXiv},
  primaryClass={cs.LG},
  url={https://arxiv.org/abs/2410.18652},
}
