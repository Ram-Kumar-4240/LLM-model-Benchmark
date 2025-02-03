# RAG with Small Models
## Overview

This project explores Retrieval-Augmented Generation (RAG) with small language models, focusing on balancing efficiency, accuracy, and performance. The goal is to evaluate the capabilities of lightweight models in retrieval-based generation tasks, benchmarking their response times, memory efficiency, and throughput to determine their suitability for real-world applications.


## Objectives
- Implement RAG (Retrieval-Augmented Generation) using small language models..
- Compare performance metrics such as response time, memory usage, and processing speed.
- Evaluate models based on their suitability for deployment in low-resource environments.
- Optimize retrieval and generation for fast and efficient outputs
- Assess trade-offs between model size and accuracy.

## Models Evaluated

The project benchmarks several small models based on speed, memory efficiency, and throughput.

| Model | Average Response Time (s) | Memory Usage (MB)| Processing Speed (tokens/sec)
| :---------- | :------- | :--------- | :--------------- |
| **Tinyllama** | **13.71** |**-0.87** |  **271.30** |
| **llama3.2** | **16.84** |**-1.71** |  **275.47** |
| **gemma2:2b** | **19.79** |**-4.03** |  **268.65** |
| **deepseek-r1:1.5b** | **24.22** |**-6.08** |  **371.40** |

![Image](https://github.com/user-attachments/assets/3af0a773-7bea-4e7f-9031-055bc2afeb35)

![Image](https://github.com/user-attachments/assets/d3368886-009d-422a-9d26-4951cd074954)

## Key Findings:
- Fastest Model: tinyllama (13.71s average response time)
- Most Memory-Efficient: deepseek-r1:1.5b (-6.08MB memory usage)
- Highest Throughput: deepseek-r1:1.5b (371.40 tokens/sec)

### Implementation Details

#### 1. Model Selection
 - Chose small-sized LLMs for low-resource environments.
 - Evaluated different architectures to compare their strengths and weaknesses

#### 2. Retrieval-Augmented Generation (RAG)
 - Integrated a retrieval mechanism to fetch relevant context before generation.
 - Used vector embeddings and a similarity search engine for optimized retrieval.
 - Combined retrieval results with LLM-generated responses to improve answer quality.

#### 3. Benchmarking
 - Measured latency, memory footprint, and token throughput.
 - Ran multiple queries per model to ensure consistent results.

#### 4. Optimization
 - Used quantization and model pruning to reduce computational costs.
 - Implemented caching mechanisms to enhance retrieval efficiency.
 - Fine-tuned hyperparameters to improve response quality.

## Use Cases
 - **Lightweight AI Assistants:** Deployable on edge devices and mobile applications. 

 - **Low-Latency Question Answering:** Efficient retrieval-based responses for real-time applications

 - **Domain-Specific RAG:** Custom knowledge integration for specialized tasks (e.g., legal, medical, finance).

## Future Enhancements
- Expand benchmarking with additional small models.
- Optimize retrieval techniques for better contextual understanding.
- Explore hybrid models that balance size and accuracy
## Conclusion
This project demonstrates the **potential of small models in RAG systems**, showing that with proper optimization, they can achieve competitive performance while being resource-efficient. The results indicate that **tinyllama** provides the fastest response time, while **deepseek-r1:1.5b** excels in memory efficiency and throughput

## Contributors
- Name : Ramkumar
- Email : infogramrk@gmail.com

