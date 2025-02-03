# RAG with Small Language Models - Benchmarking and Optimization
## Overview

This project explores Retrieval-Augmented Generation (RAG) with small language models, focusing on balancing efficiency, accuracy, and performance. The goal is to evaluate the capabilities of lightweight models in retrieval-based generation tasks, benchmarking their response times, memory efficiency, and throughput to determine their suitability for real-world applications.


## Objectives
- Implement RAG (Retrieval-Augmented Generation) using small language models..
- Compare performance metrics such as response time, memory usage, and processing speed.
- Evaluate models based on their suitability for deployment in low-resource environments.
- Optimize retrieval and generation for fast and efficient outputs
- Assess trade-offs between model size and accuracy.
## Project Scope
- Model Selection: Evaluating six small-sized LLMs, including Qwen2:1.5B, DeepSeek-R1:1.5B, Llama3.2, Gemma2:2B, Smollm2, and Granite3.1-Dense:2B.
- Retrieval Mechanism: Implementing vector search databases (e.g., FAISS, ChromaDB) for efficient knowledge retrieval.
- Benchmarking: Measuring performance based on
  - Response Time (Speed)
  - Memory Efficiency
  - Token Processing Speed
- Optimization: Identifying the best small model for RAG-based tasks without requiring excessive computational power.
## Models Evaluated

The project benchmarks several small models based on speed, memory efficiency, and throughput.

| Model | Average Response Time (s) | Memory Usage (MB)| Processing Speed (tokens/sec)
| :---------- | :------- | :--------- | :--------------- |
| **Qwen2:1.5B** | **12.70** |**0.02** |  **333.57** |
| **Granite3.1-Dense:2B** | **13.36** |**0.02** |  **373.60** |
| **Smollm2** | **13.77** |**0.03** |  **362.42** |
| **gemma2:2b** | **16.20** |**0.10** |  **329.49** |
| **deepseek-r1:1.5b** | **19.15** |**-0.53** |  **413.79** |
| **llama3.2** | **24.46** |**0.23** |  **231.39** |

![visual 3_page-0001](https://github.com/user-attachments/assets/0a9f917c-a08e-42e1-a821-6f85de017153)

![Screenshot 2025-02-03 175231](https://github.com/user-attachments/assets/c653cbe6-3f9c-4193-a42c-faf9cc26a04f)


## Key Findings:
- Fastest Model: Qwen2:1.5B (12.70s average response time).
- Most Memory-Efficient: DeepSeek-R1:1.5B (-0.53MB average memory usage).
- Highest Throughput: DeepSeek-R1:1.5B (413.79 tokens/sec).

## Technologies Used
- LLM Models: Qwen2:1.5B, DeepSeek-R1:1.5B, Llama3.2, Gemma2:2B, Smollm2, Granite3.1-Dense:2B
- Retrieval Mechanism: FAISS / ChromaDB / Weaviate (for vector-based retrieval)
- Frameworks: LangChain, Hugging Face Transformers
- Benchmarking Tools: Python scripts for profiling latency and memory usage

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

## Contributors
- Name: Ramkumar
- Email: infogramrk@gmail.com

