# Ask Mona — FAQ Chatbot

A browser-based FAQ chatbot built as part of the **CodeAlpha Artificial Intelligence Internship** (Task 2).

Powered by **Monalisa Inc. · INDIA**

## What it does

Ask Mona answers common questions about a fictional online course platform, **Monalisa Learn** — enrollment, payments, refunds, certificates, mobile access, technical support, and more.

- Type a question in plain English and get the closest matching FAQ answer
- Confident matches are answered directly; uncertain matches come with a "I think you mean..." caveat instead of a wrong guess
- If nothing matches well, it falls back to suggested questions instead of a dead end
- Quick-reply suggestion chips let you explore without typing
- Simple chat interface with a typing indicator and a clear-chat button

## How it works

- **FAQ knowledge base**: 16 question/answer pairs, each tagged with extra keywords to widen what phrasing can match them
- **Preprocessing**: incoming text and FAQ questions are lowercased, stripped of punctuation, tokenized, and filtered against a stopword list
- **Matching**: cleaned text is converted into TF-IDF weighted vectors, and the user's question is compared against every FAQ using cosine similarity — the highest-scoring FAQ (above a confidence threshold) is returned as the answer
- Pure **HTML, CSS, and JavaScript** — no backend, no build step, no API keys, and no internet connection required after the page loads

## How to run it

1. Download `ask-mona.html`
2. Open it in any modern web browser (Chrome, Edge, Firefox, Safari)
3. Start typing questions, or tap one of the suggested chips

## Tech stack

- HTML5 / CSS3
- Vanilla JavaScript — hand-rolled TF-IDF vectorization and cosine similarity (no external libraries)

## Project for

CodeAlpha Artificial Intelligence Internship — Task 2: Chatbot for FAQs
