# Memory-Augmented Agent Training for Business Document Understanding

## Overview

This repository hosts the dataset and resources associated with the paper **“Memory-Augmented Agent Training for Business Document Understanding”**, authored by Jiale Liu, Yifan Zeng, Malte Højmark-Bertelsen, Marie Normann Gadeberg, Huazheng Wang, and Qingyun Wu.

The study introduces **Matrix** (Memory-Augmented agent Training through Reasoning and Iterative eXploration), a framework enabling large language model (LLM)-based agents to iteratively learn and adapt for specialized tasks in business domains, such as extracting transport references from invoices.

## Key Contributions

1. **Matrix Framework**: A novel paradigm allowing LLM-based agents to iteratively improve reasoning and task performance by leveraging memory refinement.

2. **Open Dataset**: The first publicly available anonymized dataset for benchmarking business document understanding.

3. **Performance Gains**: Demonstrated improvements of 30–35% over existing LLM prompting and agent systems on transport reference extraction tasks.

## Dataset

The dataset includes anonymized Universal Business Language (UBL) invoice documents prepared in collaboration with Kuehne+Nagel, one of the largest logistics companies globally. The data has been anonymized to preserve document structure while protecting sensitive information.

## Dataset Features

•  **Format**: XML files containing UBL invoice documents, with a separate `ground_truth.json` file containing task annotations.

•  **Task**: Extract transport reference numbers from structured business documents.

•  **Anonymization**: All sensitive identifiers and structured data have been replaced with pseudonyms or randomized values.

### 1. Dataset Structure

The dataset is organized as follows:

```
data/
├── ground_truth.json  # Contains task annotations
├── [UUID].xml        # UBL invoice documents
```

## Results

**Method**  **Success Rate (%)**

Chain-of-Thought Prompting  18.03

Reflexion  27.28

Matrix (Proposed)  **55.82**

## Efficiency Gains

•  **30.3% improvement** over single LLM prompting methods.

•  **Reduced latency** and **fewer API calls**, making it cost-efficient for enterprise use cases.

•  Improved handling of **long documents** (up to 10,000 tokens).

## License

This repository is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

## Citation

If you use this dataset or framework, please cite the following paper:

```bibtext
@misc{liu2024memoryaugmentedagenttrainingbusiness,
      title={Memory-Augmented Agent Training for Business Document Understanding}, 
      author={Jiale Liu and Yifan Zeng and Malte Højmark-Bertelsen and Marie Normann Gadeberg and Huazheng Wang and Qingyun Wu},
      year={2024},
      eprint={2412.15274},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2412.15274}, 
}
```
  
## Contact

For questions or issues, please contact:

•  Malte Højmark-Bertelsen: [malte@beyondwork.ai](mailto:malte@beyondwork.ai)
