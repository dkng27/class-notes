# AI for everyone

## Week 1 Summary

### Supervised Learning

- Training with label
- You learned this the millionth time

### LLM in a nutshell

- Predict next word in a sentence
- Supervised Learning (have label of next word)

### Leap in performance of AI systems

- Machine Learning
- More data (Big Data)
- More compute power (dedicated hardware like GPUs)
➡️ More scalable AI performance, larger models

### Dataset

- Table of data
    - Structured data
- Data acquisition
    - Manual labelling (for supervised learning)
    - Observing behaviors, *e.g.*:
        - time, price, (target) whether purchased or not
        - temperature, pressure, (target) machine fault or not
- Many datasets are publically available

### Misuse of data

- Collecting data for new model
    - Collect small bits at a time, see if it fits AI team needs
    - Don't throw data at AI team and assume it will be valuable
    - Interplay between IT and AI teams
- More != better

### Importance of preprocessing

- Data is messy
    - Missing values
    - Incorrect labels
➡️ Data cleaning
- Mutliple type of data
    - Unstructured, images, audio, etc.

### Terminologies

- Machine Learning
    - Running AI system: website / app hosting AI for prediction
    - Software
- Data science: give a set of insights helping business decisions
    - *e.g.*, what house to build
    - Slide deck, business conclusions
- Difference between ML and DS example
    - ML: predict which ad users will click on
    - DS: which industries might be more interested in paying for ads
- Deep Learning
    - Artifical Neural Network ANN
    - Take in many params for one output

### Capabilities of ML

- "Anything you can do in 1 second of thought"
    - Chain of Thought?
- Make feasible problems for ML
  1. Concept simplicity (<= 1 sec)
  2. Data availability
  3. Data consistency

### Examples of AI

- Self-driving cars ✅
    - input: image
    - output: cars in surrounding environment
- Intention recognition ❌
    - input: hand gestures?
    - output: intention?
  ➡️ Problem too complex
        - not enough data for gestures from people
        - need high accuracy
- X-ray
    - diagnose from ~10k labelled images ✅
    - learn from a text book with only 10 images and pragraphs ❌
        - Hard to structure input A

➡️ AI performs poorly on new types of unseen data

- Changed photo format, camera angle, etc.

### Deep Learning

- Simpliest neural network, 1 neuron
    - One curve (or straight line) with decision boundary on 2D plane
- Deep learning
    - many neurons, many layers, *e.g.*
        - [price, shipping cost] -> *affordability*
        - [marketing, material] -> *perceived quality*
            - [*affordability, perceived quality*] -> **demand**
            - Intermediate concepts <mark>learned by computer itself</mark>
    - decision boundary on hyperplane
- CNN
    - For images, input image pixel brightness values
        - Black and white or RGB
