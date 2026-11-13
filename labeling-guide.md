# Intent + Sentiment Labeling Guide (EN/ES)

Each message gets **one intent** and **one sentiment**.

## Intent labels

| Label | Definition | EN example | ES example |
|---|---|---|---|
| `order_status` | Asks where an order is or when it arrives | "Where is my package?" | "¿Dónde está mi pedido?" |
| `refund_request` | Wants money back or to return an item | "I want a refund." | "Quiero que me devuelvan el dinero." |
| `product_question` | Asks about features, sizes, compatibility | "Does it come in blue?" | "¿Viene en otro color?" |
| `complaint` | Reports a problem without a specific request | "The app keeps crashing." | "La app se cierra sola." |
| `praise` | Positive feedback without a request | "Love this store!" | "¡Me encanta esta tienda!" |
| `other` | None of the above | "Hi" | "Hola" |

**Decision rule:** if a message has a complaint **and** a request, label the **request** (e.g., "It broke, I want my money back" → `refund_request`).

## Sentiment labels
`positive` · `neutral` · `negative`

## Code-switching rules
1. Label the message as a whole; never split it by language.
2. Record `language = mixed` when both languages carry meaning.
3. Slang and Spanglish ("parquear", "el delivery") are valid. Don't mark as errors.

## Regional notes
| Expression | Region | Meaning | Sentiment |
|---|---|---|---|
| "¡Qué chévere!" | Caribbean / Venezuela / Colombia | How cool | positive |
| "¡Qué guay!" | Spain | How cool | positive |
| "Me da igual" | General | I don't mind | neutral |
| "¡Qué mala onda!" | Mexico / Central America | How uncool / that's mean | negative |
