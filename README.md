### SemCoder: Semantic Awareness for Oracle and Test Generation

This project investigates the effectiveness of SemCoder, a semantic-aware code language model built on DeepSeek Coder 6.7B Instruct, in generating high-quality test cases and oracles for software testing. Building on SemCoder's novel approach to learning comprehensive program semantics. Our implementation includes a memory-optimized infrastructure for model deployment (utilizing gradient checkpointing and bfloat16 precision), a systematic evaluation pipeline for code generation assessment, and benchmarking capabilities using the HumanEval and HumanEval+ datasets.

Current progress encompasses: (1) A robust model evaluation framework with comprehensive metrics tracking, demonstrating SemCoder's strong performance with 0.7 pass@1 rate and 0.9 syntax validity; (2) Memory-efficient model loading and management systems achieving optimal performance on consumer-grade GPUs; and (3) An advanced code generation pipeline with retry mechanisms and systematic error handling. Our evaluation framework provides detailed insights into model performance across multiple dimensions, including syntax validity, execution accuracy, and test case effectiveness. Initial findings demonstrate SemCoder's significant capabilities in code generation and execution understanding, achieving 0.7 execution accuracy on our test samples. These results were validated through systematic evaluation across various HumanEval tasks, including function generation, list manipulation, and string processing.

The next phase will leverage these strong results to implement specialized prompting strategies for test case generation and oracle verification, potentially incorporating CodeDPO for further performance improvements. We plan to extend our current evaluation metrics to include test coverage analysis, edge case detection, and oracle verification accuracy, while expanding our evaluation to include more complex programming scenarios through SWE Bench verification. This research contributes to improving automated software testing practices by demonstrating the effectiveness of semantic-aware models in both code generation and validation. Our implementation is provided here as a comprehensive notebook that is fully documented with detailed comments and instructions throughout. The notebook is designed to run directly in Google Colab, requiring minimal setup and providing immediate reproducibility of our results. Each section of the notebook contains explicit setup instructions, code execution steps, and result validation processes, making our experiments easily replicable for review.