# StereoQueerEval — DL / Transfer Learning Assignment

A deep learning and transfer learning project built around the **StereoQueerEval** shared task
([SemEval-2027](https://stereoqueereval.github.io/stereoqueereval/)): detecting queer stereotypes
and hate speech in YouTube comments.

> **Note:** This repository acts as an *anchor* for the project. All actual work is done in
> **Google Colab** — this repo is where notebooks and modifications are saved and version-controlled.

## The Task

Given YouTube comments (with the parent video's title and description as context) from videos on
LGBTQIA+ topics, classify each comment across three subtasks:

| Subtask | Type | Description |
| --- | --- | --- |
| **A — Stereotype detection** | Binary | Does the comment contain a stereotype about LGBTQIA+ people? |
| **B — Hate speech classification** | Multiclass | Explicit hate / implicit hate / supportive-or-non-hateful |
| **C — Target & identity** | Multilabel | Target type (individual vs. group) and specific LGBTQIA+ identities |

### Languages

- **English** — high-resource (~2,989 instances)
- **Italian** — mid-resource, Romance (~2,400 instances)
- **Dutch** — mid-resource, Germanic (~2,238 instances)
- **Persian** — low-resource, **test phase only** (cross-lingual transfer)

The cross-lingual, low-resource Persian test set makes this a natural **transfer learning** problem.

## Data

- Format: UTF-8, tab-separated (`.tsv`), with embedded newlines handled during parsing.
- Access requires a signed **Data Usage Agreement** and joining the task's Google Group for
  archive credentials. Data is **not** committed to this repository (see `.gitignore`).
- Test sets scheduled for release **January 2027**.

## Workflow

1. Open the relevant notebook in **Google Colab**.
2. Mount data / load the dataset there (do not commit raw data).
3. Save notebook changes back to this repository (Colab → *File → Save a copy in GitHub*, or push).

## References

- Task README: <https://github.com/StereoQueerEval/StereoQueerEval_SemEval-2027>
- Official site: <https://stereoqueereval.github.io/stereoqueereval/>
