# state-metacognition-emotional-recovery-ESM

## Overview

This dataset contains a baseline questionnaire, experience sampling / diary data, and analysis files for a study of state metacognitive beliefs, emotion regulation strategies, perceived emotional recovery, and psychological distress. The diary protocol comprised 10 days with five scheduled surveys per day (50 scheduled occasions per participant).


## Folder contents

| Folder | Contents |
| --- | --- |
| `1.RawData` | Baseline (`PreESM_data.xlsx`) and diary (`ESM_data.xlsx`) data, with Chinese codebooks (`PreESM_code.xlsx`, `ESM_code.xlsx`) and English translations (`PreESM_code_EN.xlsx`, `ESM_code_EN.xlsx`). |
| `2.QuestionnaireQualityAssessment/DASS` | Filtered baseline data in Excel and SPSS format, SPSS syntax (`2.Code.sps`) for Cronbach's alpha across the 21 DASS items, and saved SPSS output (`3.Result.spv`). |
| `2.QuestionnaireQualityAssessment/Strategy_twofactors_CFA` | Mplus input, saved output, and analysis data for the multilevel two-factor confirmatory factor analysis of emotion regulation strategy indicators. |
| `3.MainResults` | Analysis data and four Mplus models: null model / ICCs, random-slope mediation, mediation including DASS total score main effects, and cross-level moderated mediation with DASS total score as moderator. |
| `4.SensitivityAnalyses` | Cross-level moderated mediation analyses using anxiety (`Anxiety`), depression (`Depression`), or stress (`Stress`) scores as the moderator. Each subfolder contains its own Mplus input, saved output, and a copy of the analysis data. |


## Usage notes

Variable definitions, response coding, and scoring procedures are provided in the codebooks in `1.RawData`.

The Mplus analysis CSV files contain no header row. Column order is specified in the corresponding `.inp` files, and missing values are coded as `-999`. Keep each `.inp` file alongside its accompanying CSV file when running the analyses.
