# DM873 · Project 1 — Cat & Dog Classification

**Deadline:** Friday 6 November 2026, 23:59 · **Hand-in:** one PDF on itslearning (one per group) · **Group size:** 3–4

🔒 [Project folder](https://drive.google.com/drive/folders/17GhmyetrZ5Wze0iUxZsICppkNUd6WqIG) · 🔒 [Project description (PDF)](https://drive.google.com/file/d/1BWiYj0hMjifppEYYTbLEIDxgWSVSl80x/view) · 🔒 [Dataset · catdog_data.zip](https://drive.google.com/file/d/1KX_BEhlCnid16CLS4qfjo_UM5OtjH8Nr/view)

## Summary

Train a deep neural network from scratch that classifies RGB JPEG images as cat or dog. The dataset is balanced (2,600 images, 1,300 per class). The report (≈3–4 pages excluding code and figures) must justify the design choices for model, regularization and evaluation, and state who did what.

**Constraints:** no pretrained networks; no training data beyond the supplied zip. Networks built during the course exercises may be reused.

## Tasks and checklist

### 1 · Data split and dataloader
- [ ] Choose train/test (or train/validation/test) proportions and justify them
- [ ] Write a custom dataloader that reads images from disk
- [ ] Apply at least one on-the-fly augmentation and justify the choice

### 2 · Network
- [ ] Design architecture, capacity and regularizers; justify each
- [ ] Plan the hyperparameter search strategy and document it
- [ ] Track parameter count (relevant for the competition)

### 3 · Visualization
- [ ] Training/validation curves
- [ ] At least one of: filters, feature maps, misclassified samples, own test photo

### Report
- [ ] 3–4 pages, code as appendix or notebook-style
- [ ] Contribution statement per group member
- [ ] Everything merged into a single PDF

## Optional competition

Ranking: best classification performance first, then the fewest parameters among the top five. Submit `competition.pth` + `competition.py` (class `competition(nn.Module)`, plus `input_dim` and `channel_dim`). The organisers' ranking script only applies `ToTensor()` and `Resize(input_dim)` — use the same preprocessing on validation/test data.

## Relevant study material

E01 (training loop), E03 (regularization, dropout, momentum), lecture 08 (regularization) — see [course page](README.md).

## Log

| Date | Who | What |
|---|---|---|
| | | |
