# AI Word Prediction — Galton Board Visualization

Interactive single-page visualization showing how Large Language Models predict the next word, using a Galton board metaphor.

A ball drops through a pyramid of words, randomly selecting the next word at each level — just like an LLM sampling from probability distributions.

## Demo

Open `index.html` in any browser. No dependencies required.

## Features

- **Galton board animation** — ball drops through 5 levels, building a sentence word by word
- **5 word groups** — click the root word to switch between different starting words (The, I, She, We, It)
- **Speed control** — slider to adjust animation speed (0.25x – 3x)
- **Step-by-step explanation** — side panel highlights each stage as the animation progresses
- **Responsive** — explanation panel stacks below on narrow screens

## How It Works

At each level, a random number (0–1) is generated:
- `< 0.5` → ball falls left
- `≥ 0.5` → ball falls right

Each path through the tree produces a different sentence. Refresh or click "Drop again" for a new random path.
