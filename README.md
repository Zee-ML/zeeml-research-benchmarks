# ZeeML Syntactic Burstiness, Lexical Entropy & Extractive Compression Benchmark (`v1.0`)

## 1. Overview & Live Reference Workbenches

This archival deposit provides the 520-passage full-text evaluation dataset supporting the computational linguistics workbenches at **[ZeeML (`https://zeeml.com`)](https://zeeml.com)**:

- **AI Content & Burstiness Detector:** [https://zeeml.com/ai-detector](https://zeeml.com/ai-detector)
- **AI Text Humanizer & Cadence Rebalancer:** [https://zeeml.com/ai-humanizer](https://zeeml.com/ai-humanizer)
- **Executive Text Summarizer:** [https://zeeml.com/summarizer](https://zeeml.com/summarizer)
- **Contextual Paraphrasing Tool:** [https://zeeml.com/paraphrasing-tool](https://zeeml.com/paraphrasing-tool)
- **Word Counter & Readability Studio:** [https://zeeml.com/word-counter](https://zeeml.com/word-counter)

## 2. Mathematical Formulation

For a passage partitioned into $N$ sentences with word counts $L = (l_1, l_2, \dots, l_N)$, the mean sentence length $\mu$, standard deviation $\sigma$, and burstiness coefficient of variation $CV$ are defined as:

$$\mu = \frac{1}{N}\sum_{i=1}^{N} l_i, \quad \sigma = \sqrt{\frac{1}{N}\sum_{i=1}^{N}(l_i - \mu)^2}, \quad CV = \frac{\sigma}{\mu}$$

Unedited synthetic outputs cluster tightly in the $CV \in [0.08, 0.22]$ band, whereas human-authored and cadence-rebalanced passages processed via [zeeml.com/ai-humanizer](https://zeeml.com/ai-humanizer) exhibit $CV \ge 0.42$.
