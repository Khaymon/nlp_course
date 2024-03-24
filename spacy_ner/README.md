## How to train
In order to train SpaCy NER model one need to run `python -m spacy train ./configs/config-01.cfg --path.train ./data/prepared/train.spacy ./data/prepared/validation.spacy`

## How to benchmark
Run `python -m spacy benchmark accuracy ./traindir/model-best ./data/prepared/test.spacy`

### Results


| Metric | Score  |
|--------|--------|
| TOK    | 100.00 |
| NER P  | 80.70  |
| NER R  | 75.30  |
| NER F  | 77.90  |
| SPEED  | 50876  |


| NER Type                | P      | R      | F      |
|-------------------------|--------|--------|--------|
| TREATMENT               | 78.74  | 69.15  | 73.64  |
| PROBLEM                 | 72.77  | 69.93  | 71.32  |
| SYSTEM_ORGAN_SITE       | 82.74  | 76.37  | 79.43  |
| DX_NAME                 | 86.30  | 86.72  | 86.51  |
| GENERIC_NAME            | 78.44  | 75.82  | 77.11  |
| TEST                    | 64.29  | 53.39  | 58.33  |
| TREATMENT_NAME          | 75.79  | 49.35  | 59.78  |
| NUMBER                  | 92.99  | 97.16  | 95.03  |
| BRAND_NAME              | 48.70  | 30.70  | 37.66  |
| NAME                    | 0.00   | 0.00   | 0.00   |
| TEST_NAME               | 56.25  | 38.03  | 45.38  |
| PROCEDURE_NAME          | 60.38  | 56.14  | 58.18  |
| TIME_TO_TREATMENT_NAME  | 0.00   | 0.00   | 0.00   |
| AGE                     | 80.95  | 36.96  | 50.75  |
| TIME_TO_DX_NAME         | 66.67  | 15.38  | 25.00  |
| TIME_TO_MEDICATION_NAME | 21.43  | 17.65  | 19.35  |
| ADDRESS                 | 93.75  | 57.69  | 71.43  |
| DATE                    | 0.00   | 0.00   | 0.00   |
| TIME_TO_TEST_NAME       | 75.00  | 30.00  | 42.86  |
| TIME_TO_PROCEDURE_NAME  | 0.00   | 0.00   | 0.00   |
| PROFESSION              | 0.00   | 0.00   | 0.00   |
