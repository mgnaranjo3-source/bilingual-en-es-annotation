# Bilingual EN/ES Annotation Samples

Sample guidelines and labeled data for **English–Spanish** annotation tasks: intent and sentiment labeling, code-switched text, and translation quality review.

> All texts in this repo are **synthetic**, written for demonstration. No real users, customers or project data.

## Why bilingual annotation needs its own rules

- **Code-switching** ("el delivery llegó late otra vez") is normal speech, not an error, and must be labeled as one text.
- **Regional variation** (Mexico, Caribbean, Spain, South America) changes meaning: *"¡Qué chévere!"* vs *"¡Qué guay!"* both mean "how cool".
- **Literal translation hides intent**: *"No hay de qué"* is "you're welcome", not "there is nothing".
- **Formality** (*tú* vs *usted*) can be part of a style requirement in AI responses.

## Contents

| File | Purpose |
|---|---|
| [`labeling-guide.md`](labeling-guide.md) | Intent + sentiment label set with EN/ES examples and code-switching rules |
| [`data/intent_sentiment_samples.csv`](data/intent_sentiment_samples.csv) | 20 labeled synthetic messages (EN, ES, mixed) |
| [`translation-review.md`](translation-review.md) | Error categories and severity scale for reviewing EN↔ES translations, with examples |

## License

MIT
