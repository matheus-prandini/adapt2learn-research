# Gael + Financial Mathematics — Questionnaires and Response Data

This directory contains the data collection instruments and the anonymized
response data for the study:

> **Student Engagement and Perceived Learning in an Educational Platform Game
> with Automatic Question Generation: A Brazilian High School Study**
> (SBGames 2026, Full Papers — Education Track).

The study is an exploratory case study of *Gael*, a 2D educational platform
game coupled with an automatic multiple-choice question generation module,
deployed in financial-education lessons with 11th-grade students at a Brazilian
public high school.

---

## Repository placement

This dataset is released as part of the **`adapt2learn-research`** repository.
Because that repository is an umbrella for several studies, this material lives
in its own self-contained study folder:

```
adapt2learn-research/
└── data-release/
    └── sbgames-2026-gael-financial-math/
        ├── README.md                              # this file
        ├── data/
        │   ├── student_questionnaire_responses.csv
        │   └── teacher_questionnaire_responses.csv
        └── instruments/
            ├── student_questionnaire.pdf           # blank form (to be added)
            └── teacher_questionnaire.pdf           # blank form (to be added)
```

The stable link cited in the paper should point to this folder (or to the
archived release / DOI that contains it).

---

## Files

| File | Description | Rows (responses) |
|------|-------------|------------------|
| `data/student_questionnaire_responses.csv` | Student post-session questionnaire | 61 |
| `data/teacher_questionnaire_responses.csv` | Teacher questionnaire | see note below |
| `instruments/*.pdf` | Blank questionnaire forms | — |

**Language.** All items and open-ended answers are in **Brazilian Portuguese**,
as administered. Column headers are the verbatim questionnaire items.

**Format.** UTF-8 CSV, comma-separated, one response per row. Multi-line
open-ended answers are enclosed in double quotes.

---

## Likert scale

All closed items use a 5-point Likert scale. Values are stored as text in the
original Portuguese wording and map to numeric scores as follows:

| Stored value | Score | English |
|--------------|:-----:|---------|
| `1 – Discordo totalmente` | 1 | Strongly disagree |
| `2 – Discordo` | 2 | Disagree |
| `3 – Nem concordo nem discordo` | 3 | Neither agree nor disagree |
| `4 – Concordo` | 4 | Agree |
| `5 – Concordo totalmente` | 5 | Strongly agree |

---

## Data dictionary — student questionnaire

14 columns: 1 timestamp + 10 Likert items + 3 open-ended questions.

| # | Column (Portuguese, abbreviated) | Construct | Type |
|---|----------------------------------|-----------|------|
| 1 | Carimbo de data/hora | Submission timestamp | datetime |
| 2 | O jogo Gael foi divertido de jogar | Fun / Enjoyment | Likert 1–5 |
| 3 | Eu entendi o que precisava fazer | Usability — understood what to do | Likert 1–5 |
| 4 | Os comandos e controles foram fáceis de usar | Usability — controls easy | Likert 1–5 |
| 5 | Os desafios de raciocínio foram interessantes | Content — reasoning challenges interesting | Likert 1–5 |
| 6 | As perguntas de conteúdo fizeram sentido | Content — math questions made sense | Likert 1–5 |
| 7 | O nível de dificuldade foi adequado | Content — difficulty adequate | Likert 1–5 |
| 8 | Fiquei atento/concentrado na atividade | Attention / Engagement | Likert 1–5 |
| 9 | O jogo me ajudou a rever/aprender o conteúdo | Perceived learning | Likert 1–5 |
| 10 | Me senti motivado a continuar jogando | Motivation | Likert 1–5 |
| 11 | Gostaria de usar o Gael novamente | Reuse intention | Likert 1–5 |
| 12 | O que você mais gostou no jogo? | Open-ended — likes | text |
| 13 | O que você menos gostou / achou mais difícil? | Open-ended — dislikes / difficulties | text |
| 14 | De que forma o jogo ajudou (ou não) neste conteúdo? | Open-ended — perceived learning contribution | text |

---

## Data dictionary — teacher questionnaire

11 columns: 1 timestamp + 7 Likert items + 3 open-ended questions.

| # | Column (Portuguese, abbreviated) | Construct | Type |
|---|----------------------------------|-----------|------|
| 1 | Carimbo de data/hora | Submission timestamp | datetime |
| 2 | O jogo pareceu engajar a turma | Engagement | Likert 1–5 |
| 3 | Esteve alinhado ao nível adequado | Alignment with grade level | Likert 1–5 |
| 4 | Foi viável no tempo de aula | Feasibility | Likert 1–5 |
| 5 | Alunos mais motivados que em atividades tradicionais | Motivation vs. traditional activities | Likert 1–5 |
| 6 | Ajudou os alunos a compreender/revisar o conteúdo | Learning support | Likert 1–5 |
| 7 | Me senti confortável em mediar a atividade | Comfort mediating | Likert 1–5 |
| 8 | Vejo potencial de uso futuro | Future-use potential | Likert 1–5 |
| 9 | Principais pontos fortes | Open-ended — strengths | text |
| 10 | Principais desafios / limitações | Open-ended — challenges | text |
| 11 | Sugestões de melhoria | Open-ended — suggestions | text |

---

## Note on the teacher responses

The teacher file contains responses from the mathematics teachers who
accompanied the intervention. The statistics reported in the paper are based on
the **two mathematics teachers who attended all three gameplay sessions**
(the responses submitted on 24 Apr 2026). Any additional, later response
included in the raw file was **not** part of the analysis reported in the paper
and is provided only for completeness/transparency.

> If you prefer to distribute only the analyzed responses, keep the two
> 24 Apr 2026 rows in `teacher_questionnaire_responses.csv` and remove the
> later one; then update this note accordingly.

---

## Sample and ethics

- **Students:** final analytic sample of **N = 61** (from three 11th-grade
  classes; students who missed any of the three sessions were excluded).
- **Anonymization:** the forms did **not** collect names, e-mail addresses,
  student IDs, or any other direct identifier. Each row contains only a
  submission timestamp and the answers. No personally identifiable information
  is present.
- All participants took part under informed consent, and the study received
  ethics-committee approval (see the paper for details).

---

## License

Unless stated otherwise, this data and documentation are released under the
**Creative Commons Attribution 4.0 International (CC BY 4.0)** license,
consistent with the publication. You are free to share and adapt the material
with appropriate credit.

---

## How to cite

> *(Add the full paper reference / DOI once the proceedings are published.)*

## Contact

> *(Add corresponding-author contact for questions about the data.)*
