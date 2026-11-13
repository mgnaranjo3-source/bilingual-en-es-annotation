# EN ↔ ES Translation Review

A simple error typology for reviewing machine or human translations, inspired by common MQM-style practice.

## Error categories

| Category | What it means |
|---|---|
| **Accuracy – mistranslation** | Meaning changed |
| **Accuracy – omission / addition** | Content dropped or invented |
| **Fluency – grammar** | Agreement, tense, gender errors |
| **Fluency – spelling / punctuation** | Missing accents, wrong ¿¡ usage |
| **Style – register** | Wrong formality (tú/usted) for the context |
| **Locale** | Wrong date/number/currency format or regional term |
| **Terminology** | Domain term translated inconsistently or wrongly |

## Severity
| Severity | Definition | Points |
|---|---|---|
| Critical | Could cause harm, legal or safety risk, or totally wrong meaning | 10 |
| Major | Meaning is affected; reader may be misled | 5 |
| Minor | Meaning intact, but quality is lower | 1 |

## Worked examples (synthetic)

| Source (EN) | Translation (ES) | Issue | Category | Severity | Correct version |
|---|---|---|---|---|---|
| "Take one tablet twice a day." | "Tome dos tabletas una vez al día." | Dose reversed | Accuracy – mistranslation | Critical | "Tome una tableta dos veces al día." |
| "Your order ships on 03/04." (US date) | "Su pedido se envía el 03/04." | Ambiguous date for ES readers (3 April vs 4 March) | Locale | Major | "Su pedido se envía el 4 de marzo." |
| "Hey! Check out our new deals." (casual brand) | "Estimado cliente, consulte nuestras nuevas ofertas." | Too formal for brand voice | Style – register | Minor | "¡Hola! Mira nuestras nuevas ofertas." |
| "Embarrassed" | "Embarazada" | False friend (means *pregnant*) | Accuracy – mistranslation | Major | "Avergonzado/a" |
| "How are you?" | "Como estas?" | Missing accents and opening ¿ | Fluency – spelling | Minor | "¿Cómo estás?" |
