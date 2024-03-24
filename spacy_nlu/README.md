# Intents classification
Intents classification using rule-based methods and with trained from scratch model.

## Training from scratch

### Data preparation

We split ATIS intents dataset for train, val and test parts with ratios `0.8`, `0.1` and `0.1` respectfully.

### How to train

Run `python -m spacy train ./configs/config-01.cfg --paths.train ./data/prepared/train.spacy --paths.dev ./data/prepared/val.spacy --output ./traindir`

### How to benchmark
Run `python -m spacy benchmark accuracy ./traindir/model-best ./data/prepared/test.spacy`

### Results

| Metric              | Score  |
| ------------------- | ------ |
| TOK                 | 100.00 |
| TEXTCAT (macro AUC) | 73.56  |
| SPEED               | 110624 |

| Textcat Label        | P       | R       | F       |
|----------------------|---------|---------|---------|
| atis_flight_time     | 100.00  | 71.43   | 83.33   |
| atis_ground_fare     | 0.00    | 0.00    | 0.00    |
| atis_airfare         | 95.56   | 95.56   | 95.56   |
| atis_flight          | 98.92   | 98.65   | 98.78   |
| atis_aircraft        | 60.00   | 85.71   | 70.59   |
| atis_capacity        | 100.00  | 50.00   | 66.67   |
| atis_airport         | 50.00   | 100.00  | 66.67   |
| atis_distance        | 100.00  | 100.00  | 100.00  |
| atis_flight_no       | 0.00    | 0.00    | 0.00    |
| atis_restriction     | 0.00    | 0.00    | 0.00    |
| atis_city            | 100.00  | 50.00   | 66.67   |
| atis_cheapest        | 0.00    | 0.00    | 0.00    |
| atis_abbreviation    | 90.91   | 100.00  | 95.24   |
| atis_airline         | 100.00  | 90.91   | 95.24   |
| atis_ground_service  | 96.15   | 96.15   | 96.15   |
| atis_meal            | 0.00    | 0.00    | 0.00    |
| atis_quantity        | 100.00  | 100.00  | 100.00  |


| Textcat Label          | ROC AUC |
|------------------------|---------|
| atis_flight_time       | 0.87    |
| atis_ground_fare       | 0.67    |
| atis_airfare           | 1.00    |
| atis_flight            | 1.00    |
| atis_aircraft          | 0.99    |
| atis_capacity          | 1.00    |
| atis_airport           | 1.00    |
| atis_distance          | 1.00    |
| atis_flight_no         | None    |
| atis_restriction       | None    |
| atis_city              | 0.99    |
| atis_cheapest          | None    |
| atis_abbreviation      | 1.00    |
| atis_airline           | 0.99    |
| atis_ground_service    | 1.00    |
| atis_meal              | None    |
| atis_quantity          | 1.00    |
