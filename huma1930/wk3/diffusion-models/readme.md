# Text-to-Image Models

## What is

Reverse of auto labelling (get description from images) in 2015 → enter text description prompt to generate images (bruh)

➡ Prompt engineering: enter in specific key words to get generated results you want

## Examples

- Dall.E (OpenAI)
- MidJourney (Community)

## Steps

1. Deep learning
    - Images and captions (alt text) scrapped from Internet
    - Learn corresponding between image pixel values and label
2. Latent space
    - High dimensional mathematical space separating different concepts
    - For diffusion models, ~50 dimensions
    - Each point is a 50-coordinate point inside latent space
3. Diffusion
    - Start with noise
    - Arranging pixels to human recognizable format over iterations
    - Random process

## Challenges

- Biases
    - Old white guy as CEO, "Asian" keyword leads to porn images (?)
    - Copyright of images from training data
        - James Gurney, an artist that is open to GenAI images, think that the <mark>prompts and software</mark> should be mentioned
    - Unknown bad data in dataset ("dark corners")
