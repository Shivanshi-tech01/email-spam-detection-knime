# Email Spam Detection Using Machine Learning (KNIME)

Classifies SMS/email messages as spam or ham using a Decision Tree in KNIME Analytics Platform.

## Workflow
CSV Reader → Strings to Document → Text Preprocessing (Punctuation Erasure, Number Filter, Case Converter, Stop Word Filter, Snowball Stemmer, N Chars Filter) → Bag Of Words Creator → Document Vector → Category to Class → Column Filter → Table Partitioner (70/30) → Decision Tree Learner → Decision Tree Predictor → Scorer

## Results (test set, 50 messages)
- Accuracy: 86%
- Spam precision: 0.963
- Spam recall: 0.812
- F-measure (spam): 0.881

## Files
- `Spam_detection.knwf` : KNIME workflow (File > Import KNIME Workflow to open)
- `spam_sample_dataset.csv` : labeled dataset (168 messages)
- `Technical_Report.pdf` : full technical report
- `screenshots/` : workflow and results screenshots

## Author
Shivanshi Vishwakarma
