# DEPRECATED - Updates and contributions

This repository is now depracated and won't be getting any new updates. For contributions and corrections of the data seen in [LLM Stats](https://llm-stats.com/) please create a post with the tag "Issue" in the [official community section](https://llm-stats.com/posts) of the website.

For model and/or benchmark specific corrections, please visit create an Issue under the "Discussion" tab of the model/benchmark, as seen in the example below.

<img width="1156" height="575" alt="Screenshot 2025-10-24 at 1 43 52 p m" src="https://github.com/user-attachments/assets/b78f2cf3-f3ff-4a51-bba4-d8643865d16b" />

---

<img width="1208" alt="image" src="https://github.com/user-attachments/assets/835f1e1b-73e6-405a-b7ad-096d5f5f567a" />

# LLM-Stats.com

[![GitHub stars](https://img.shields.io/github/stars/JonathanChavezTamales/llm-leaderboard?style=social)](https://github.com/JonathanChavezTamales/llm-leaderboard/stargazers)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Discord](https://img.shields.io/badge/Discord-Join%20Us-7289da?logo=discord&logoColor=white)](https://discord.com/invite/RxGUBvE42d)
[![Issues](https://img.shields.io/github/issues/JonathanChavezTamales/llm-leaderboard)](https://github.com/JonathanChavezTamales/llm-leaderboard/issues)

A community-driven repository of LLM data and benchmarks. Compare and explore language models through our interactive dashboard at [llm-stats.com](https://llm-stats.com).

## Found an issue or have a feature request?

[Open an issue here](https://github.com/JonathanChavezTamales/llm-leaderboard/issues). Thank you!

# Data

## 🔍 What's Inside

Our repository contains detailed information on hundreds of LLMs:

- Model parameters, context window sizes, licensing details, capabilities, and more
- Provider pricing and configurations
- Performance metrics (throughput, latency)
- Standardized benchmark results
- Organization and license information

## 📁 Data Structure

All data is organized in the `data/` directory:

- `data/models/` - Model metadata and configurations
- `data/providers/` - Provider information
- `data/provider_models/` - Provider-specific model pricing and features
- `data/benchmarks/` - Benchmark definitions
- `data/model_benchmarks/` - Model benchmark scores
- `data/organizations/` - Organization information
- `data/licenses/` - License definitions

## 🤝 How to Contribute

We welcome community contributions to keep our data accurate and up-to-date:

1. **Update Model Data**

   - Browse the [`data/`](data/) directory structure
   - Submit a PR following our [contribution guidelines](CONTRIBUTING.md)
   - Check [`schemas/`](schemas/) for JSON Schema validation

## 📈 Data Quality

Accuracy is our priority. To ensure reliable information:

- All benchmark data requires verifiable source links
- Community review process for all changes
- Multiple source citations encouraged
- Regular validation of submitted data

There's no guarantee that the data is 100% accurate, but we do our best to ensure it's as accurate as possible.

## 🌟 Community

- Join our [Discord](https://discord.gg/RxGUBvE42d) for discussions

## Leaderboard

| Name                                     | Release Date | Input Context | Output Context | GPQA  | MMLU  | MMLU-Pro | MATH  | HumanEval | MMMU  | LiveCodeBench |
| ---------------------------------------- | ------------ | ------------- | -------------- | ----- | ----- | -------- | ----- | --------- | ----- | ------------- |
| GPT-5                                    | 2025-08-07   | N/A           | N/A            | 0.857 | 0.925 | N/A      | 0.847 | 0.934     | 0.842 | N/A           |
| o1                                       | 2024-12-17   | N/A           | N/A            | 0.780 | 0.918 | N/A      | 0.964 | 0.881     | 0.776 | N/A           |
| GPT-4.5                                  | 2025-02-27   | N/A           | N/A            | 0.695 | 0.908 | N/A      | N/A   | 0.880     | 0.752 | N/A           |
| o1-preview                               | 2024-09-12   | N/A           | N/A            | 0.733 | 0.908 | N/A      | 0.855 | N/A       | N/A   | N/A           |
| Claude 3.5 Sonnet                        | 2024-10-22   | N/A           | N/A            | 0.672 | 0.904 | 0.776    | 0.783 | 0.937     | 0.683 | N/A           |
| Claude 3.5 Sonnet                        | 2024-06-21   | N/A           | N/A            | 0.594 | 0.904 | 0.761    | 0.711 | 0.920     | N/A   | N/A           |
| Kimi K2 0905                             | 2025-09-05   | N/A           | N/A            | 0.758 | 0.902 | 0.825    | 0.891 | 0.945     | N/A   | N/A           |
| GPT-4.1                                  | 2025-04-14   | N/A           | N/A            | 0.663 | 0.902 | N/A      | N/A   | N/A       | 0.748 | N/A           |
| Kimi K2 Instruct                         | 2025-07-11   | N/A           | N/A            | 0.751 | 0.895 | 0.811    | N/A   | 0.933     | N/A   | N/A           |
| GPT-4o                                   | 2024-05-13   | N/A           | N/A            | 0.536 | 0.887 | 0.726    | 0.766 | 0.902     | N/A   | N/A           |
| DeepSeek-V3                              | 2024-12-25   | N/A           | N/A            | 0.591 | 0.885 | 0.759    | N/A   | N/A       | N/A   | 0.376         |
| Qwen3 235B A22B                          | 2025-04-29   | N/A           | N/A            | 0.475 | 0.878 | 0.682    | 0.718 | N/A       | N/A   | 0.707         |
| Kimi K2 Base                             | 2025-07-11   | N/A           | N/A            | 0.481 | 0.878 | 0.692    | 0.702 | N/A       | N/A   | N/A           |
| Grok-2                                   | 2024-08-13   | N/A           | N/A            | 0.560 | 0.875 | 0.755    | 0.761 | 0.884     | 0.661 | N/A           |
| GPT-4.1 mini                             | 2025-04-14   | N/A           | N/A            | 0.650 | 0.875 | N/A      | N/A   | N/A       | 0.727 | N/A           |
| Kimi-k1.5                                | 2025-01-20   | N/A           | N/A            | N/A   | 0.874 | N/A      | N/A   | N/A       | 0.700 | N/A           |
| Llama 3.1 405B Instruct                  | 2024-07-23   | N/A           | N/A            | 0.507 | 0.873 | 0.733    | 0.738 | 0.890     | N/A   | N/A           |
| o3-mini                                  | 2025-01-30   | N/A           | N/A            | 0.772 | 0.869 | N/A      | 0.979 | N/A       | N/A   | N/A           |
| Claude 3 Opus                            | 2024-02-29   | N/A           | N/A            | 0.504 | 0.868 | 0.685    | 0.601 | 0.849     | N/A   | N/A           |
| GPT-4 Turbo                              | 2024-04-09   | N/A           | N/A            | 0.480 | 0.865 | N/A      | 0.726 | 0.871     | N/A   | N/A           |
| GPT-4                                    | 2023-06-13   | N/A           | N/A            | 0.357 | 0.864 | N/A      | 0.420 | 0.670     | N/A   | N/A           |
| Grok-2 mini                              | 2024-08-13   | N/A           | N/A            | 0.510 | 0.862 | 0.720    | 0.730 | 0.857     | 0.632 | N/A           |
| Llama 3.2 90B Instruct                   | 2024-09-25   | N/A           | N/A            | 0.467 | 0.860 | N/A      | 0.680 | N/A       | 0.603 | N/A           |
| Llama 3.3 70B Instruct                   | 2024-12-06   | N/A           | N/A            | 0.505 | 0.860 | 0.689    | 0.770 | 0.884     | N/A   | N/A           |
| Nova Pro                                 | 2024-11-20   | N/A           | N/A            | 0.469 | 0.859 | N/A      | 0.766 | 0.890     | 0.617 | N/A           |
| Gemini 1.5 Pro                           | 2024-05-01   | N/A           | N/A            | 0.591 | 0.859 | 0.758    | 0.865 | 0.841     | 0.659 | N/A           |
| GPT-4o                                   | 2024-08-06   | N/A           | N/A            | 0.701 | 0.857 | 0.747    | N/A   | N/A       | 0.722 | N/A           |
| Llama 4 Maverick                         | 2025-04-05   | N/A           | N/A            | 0.698 | 0.855 | 0.805    | 0.612 | N/A       | 0.734 | 0.434         |
| o1-mini                                  | 2024-09-12   | N/A           | N/A            | 0.600 | 0.852 | N/A      | N/A   | 0.924     | N/A   | N/A           |
| Phi 4                                    | 2024-12-12   | N/A           | N/A            | 0.561 | 0.848 | 0.704    | 0.804 | 0.826     | N/A   | N/A           |
| Mistral Large 2                          | 2024-07-24   | N/A           | N/A            | N/A   | 0.840 | N/A      | N/A   | 0.920     | N/A   | N/A           |
| Llama 3.1 70B Instruct                   | 2024-07-23   | N/A           | N/A            | 0.417 | 0.836 | 0.664    | N/A   | 0.805     | N/A   | N/A           |
| Qwen2.5 32B Instruct                     | 2024-09-19   | N/A           | N/A            | 0.495 | 0.833 | 0.690    | 0.831 | 0.884     | N/A   | N/A           |
| Qwen2 72B Instruct                       | 2024-07-23   | N/A           | N/A            | 0.424 | 0.823 | 0.644    | 0.597 | 0.860     | N/A   | N/A           |
| GPT-4o mini                              | 2024-07-18   | N/A           | N/A            | 0.402 | 0.820 | N/A      | 0.702 | 0.872     | 0.594 | N/A           |
| Grok-1.5                                 | 2024-03-28   | N/A           | N/A            | 0.359 | 0.813 | 0.510    | 0.506 | 0.741     | 0.536 | N/A           |
| Jamba 1.5 Large                          | 2024-08-22   | N/A           | N/A            | 0.369 | 0.812 | 0.535    | N/A   | N/A       | N/A   | N/A           |
| Mistral Small 3.1 24B Base               | 2025-03-17   | N/A           | N/A            | 0.375 | 0.810 | 0.560    | N/A   | N/A       | 0.593 | N/A           |
| Mistral Small 3 24B Base                 | 2025-01-30   | N/A           | N/A            | 0.344 | 0.807 | 0.544    | 0.460 | N/A       | N/A   | N/A           |
| Mistral Small 3.1 24B Instruct           | 2025-03-17   | N/A           | N/A            | 0.460 | 0.806 | 0.668    | 0.693 | 0.884     | 0.593 | N/A           |
| Nova Lite                                | 2024-11-20   | N/A           | N/A            | 0.420 | 0.805 | N/A      | 0.733 | 0.854     | 0.562 | N/A           |
| Mistral Small 3.2 24B Instruct           | 2025-06-20   | N/A           | N/A            | 0.461 | 0.805 | 0.691    | 0.694 | N/A       | 0.625 | N/A           |
| DeepSeek-V2.5                            | 2024-05-08   | N/A           | N/A            | N/A   | 0.804 | N/A      | 0.747 | 0.890     | N/A   | N/A           |
| Llama 3.1 Nemotron 70B Instruct          | 2024-10-01   | N/A           | N/A            | N/A   | 0.802 | N/A      | N/A   | N/A       | N/A   | N/A           |
| GPT-4.1 nano                             | 2025-04-14   | N/A           | N/A            | 0.503 | 0.801 | N/A      | N/A   | N/A       | 0.554 | N/A           |
| Qwen2.5 14B Instruct                     | 2024-09-19   | N/A           | N/A            | 0.455 | 0.797 | 0.637    | 0.800 | 0.835     | N/A   | N/A           |
| Llama 4 Scout                            | 2025-04-05   | N/A           | N/A            | 0.572 | 0.796 | 0.743    | 0.503 | N/A       | 0.694 | 0.328         |
| Claude 3 Sonnet                          | 2024-02-29   | N/A           | N/A            | 0.404 | 0.790 | 0.568    | 0.431 | 0.730     | N/A   | N/A           |
| Gemini 1.5 Flash                         | 2024-05-01   | N/A           | N/A            | 0.510 | 0.789 | 0.673    | 0.779 | 0.743     | 0.623 | N/A           |
| Phi-3.5-MoE-instruct                     | 2024-08-23   | N/A           | N/A            | 0.368 | 0.789 | 0.453    | 0.595 | 0.707     | N/A   | N/A           |
| Qwen2.5 VL 32B Instruct                  | 2025-02-28   | N/A           | N/A            | 0.460 | 0.784 | 0.688    | 0.822 | 0.915     | 0.700 | N/A           |
| Nova Micro                               | 2024-11-20   | N/A           | N/A            | 0.400 | 0.776 | N/A      | 0.693 | 0.811     | N/A   | N/A           |
| Command R+                               | 2024-08-30   | N/A           | N/A            | N/A   | 0.757 | N/A      | N/A   | N/A       | N/A   | N/A           |
| Gemma 2 27B                              | 2024-06-27   | N/A           | N/A            | N/A   | 0.752 | N/A      | 0.423 | 0.518     | N/A   | N/A           |
| Claude 3 Haiku                           | 2024-03-13   | N/A           | N/A            | 0.333 | 0.752 | N/A      | 0.389 | 0.759     | N/A   | N/A           |
| Qwen2.5-Coder 32B Instruct               | 2024-09-19   | N/A           | N/A            | N/A   | 0.751 | 0.504    | 0.572 | 0.927     | N/A   | 0.314         |
| Llama 3.2 11B Instruct                   | 2024-09-25   | N/A           | N/A            | 0.328 | 0.730 | N/A      | 0.519 | N/A       | 0.507 | N/A           |
| Gemini 1.0 Pro                           | 2024-02-15   | N/A           | N/A            | 0.279 | 0.718 | N/A      | 0.326 | N/A       | 0.479 | N/A           |
| Gemma 2 9B                               | 2024-06-27   | N/A           | N/A            | N/A   | 0.713 | N/A      | 0.366 | 0.402     | N/A   | N/A           |
| Qwen2 7B Instruct                        | 2024-07-23   | N/A           | N/A            | 0.253 | 0.705 | 0.441    | 0.496 | 0.799     | N/A   | 0.266         |
| GPT-3.5 Turbo                            | 2023-03-21   | N/A           | N/A            | 0.308 | 0.698 | N/A      | 0.431 | 0.680     | 0.000 | N/A           |
| Jamba 1.5 Mini                           | 2024-08-22   | N/A           | N/A            | 0.323 | 0.697 | 0.425    | N/A   | N/A       | N/A   | N/A           |
| Llama 3.1 8B Instruct                    | 2024-07-23   | N/A           | N/A            | 0.304 | 0.694 | 0.483    | N/A   | 0.726     | N/A   | N/A           |
| Pixtral-12B                              | 2024-09-17   | N/A           | N/A            | N/A   | 0.692 | N/A      | 0.481 | 0.720     | 0.525 | N/A           |
| Phi-3.5-mini-instruct                    | 2024-08-23   | N/A           | N/A            | 0.304 | 0.690 | 0.474    | 0.485 | 0.628     | N/A   | N/A           |
| Mistral NeMo Instruct                    | 2024-07-18   | N/A           | N/A            | N/A   | 0.680 | N/A      | N/A   | N/A       | N/A   | N/A           |
| Qwen2.5-Coder 7B Instruct                | 2024-09-19   | N/A           | N/A            | N/A   | 0.676 | 0.401    | 0.466 | 0.884     | N/A   | 0.182         |
| Phi 4 Mini                               | 2025-02-01   | N/A           | N/A            | 0.252 | 0.673 | 0.528    | 0.640 | N/A       | N/A   | N/A           |
| Granite 3.3 8B Instruct                  | 2025-04-16   | N/A           | N/A            | N/A   | 0.655 | N/A      | N/A   | 0.897     | N/A   | N/A           |
| Ministral 8B Instruct                    | 2024-10-16   | N/A           | N/A            | N/A   | 0.650 | N/A      | 0.545 | 0.348     | N/A   | N/A           |
| Gemma 3n E4B Instructed LiteRT Preview   | 2025-05-20   | N/A           | N/A            | 0.237 | 0.649 | 0.506    | N/A   | 0.750     | N/A   | 0.132         |
| Gemma 3n E4B Instructed                  | 2025-06-26   | N/A           | N/A            | 0.237 | 0.649 | 0.506    | N/A   | 0.750     | N/A   | 0.132         |
| Granite 3.3 8B Base                      | 2025-04-16   | N/A           | N/A            | N/A   | 0.639 | N/A      | N/A   | 0.897     | N/A   | N/A           |
| Llama 3.2 3B Instruct                    | 2024-09-25   | N/A           | N/A            | 0.328 | 0.634 | N/A      | 0.480 | N/A       | N/A   | N/A           |
| IBM Granite 4.0 Tiny Preview             | 2025-05-02   | N/A           | N/A            | N/A   | 0.604 | N/A      | N/A   | 0.824     | N/A   | N/A           |
| Gemma 3n E2B Instructed LiteRT (Preview) | 2025-05-20   | N/A           | N/A            | 0.248 | 0.601 | 0.405    | N/A   | 0.665     | N/A   | 0.132         |
| Gemma 3n E2B Instructed                  | 2025-06-26   | N/A           | N/A            | 0.248 | 0.601 | 0.405    | N/A   | 0.665     | N/A   | 0.132         |
| Kimi K2-Instruct-0905                    | 2025-09-05   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Gemma 3n E4B                             | 2025-06-26   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Gemma 3 12B                              | 2025-03-12   | N/A           | N/A            | 0.409 | N/A   | 0.606    | 0.838 | 0.854     | N/A   | 0.246         |
| Gemini 2.5 Pro                           | 2025-05-20   | N/A           | N/A            | 0.830 | N/A   | N/A      | N/A   | N/A       | 0.796 | N/A           |
| Gemini 2.0 Flash-Lite                    | 2025-02-05   | N/A           | N/A            | 0.515 | N/A   | 0.716    | 0.868 | N/A       | 0.680 | N/A           |
| Gemini 2.5 Flash-Lite                    | 2025-06-17   | N/A           | N/A            | 0.646 | N/A   | N/A      | N/A   | N/A       | 0.729 | 0.337         |
| Gemini 2.5 Pro Preview 06-05             | 2025-06-05   | N/A           | N/A            | 0.864 | N/A   | N/A      | N/A   | N/A       | 0.820 | 0.690         |
| Gemini 2.5 Flash                         | 2025-05-20   | N/A           | N/A            | 0.828 | N/A   | N/A      | N/A   | N/A       | 0.797 | N/A           |
| Gemini 2.0 Flash Thinking                | 2025-01-21   | N/A           | N/A            | 0.742 | N/A   | N/A      | N/A   | N/A       | 0.754 | N/A           |
| Gemma 3n E2B                             | 2025-06-26   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| MedGemma 4B IT                           | 2025-05-20   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Gemma 3 4B                               | 2025-03-12   | N/A           | N/A            | 0.308 | N/A   | 0.436    | 0.756 | 0.713     | N/A   | 0.126         |
| Gemma 3 27B                              | 2025-03-12   | N/A           | N/A            | 0.424 | N/A   | 0.675    | 0.890 | 0.878     | N/A   | 0.297         |
| Gemma 3 1B                               | 2025-03-12   | N/A           | N/A            | 0.192 | N/A   | 0.147    | 0.480 | 0.415     | N/A   | 0.019         |
| Gemini 1.5 Flash 8B                      | 2024-03-15   | N/A           | N/A            | 0.384 | N/A   | 0.587    | 0.587 | N/A       | 0.537 | N/A           |
| Gemini Diffusion                         | 2025-05-20   | N/A           | N/A            | 0.404 | N/A   | N/A      | N/A   | 0.896     | N/A   | 0.309         |
| Gemini 2.0 Flash                         | 2024-12-01   | N/A           | N/A            | 0.621 | N/A   | 0.764    | 0.897 | N/A       | 0.707 | 0.351         |
| Phi 4 Mini Reasoning                     | 2025-04-30   | N/A           | N/A            | 0.520 | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Phi-3.5-vision-instruct                  | 2024-08-23   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | 0.430 | N/A           |
| Phi 4 Reasoning Plus                     | 2025-04-30   | N/A           | N/A            | 0.689 | N/A   | 0.760    | N/A   | N/A       | N/A   | 0.531         |
| Phi-4-multimodal-instruct                | 2025-02-01   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | 0.551 | N/A           |
| Phi 4 Reasoning                          | 2025-04-30   | N/A           | N/A            | 0.658 | N/A   | 0.743    | N/A   | N/A       | N/A   | 0.538         |
| Qwen3-235B-A22B-Instruct-2507            | 2025-07-22   | N/A           | N/A            | 0.775 | N/A   | 0.830    | N/A   | N/A       | N/A   | N/A           |
| QwQ-32B                                  | 2025-03-05   | N/A           | N/A            | 0.652 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.634         |
| Qwen3-235B-A22B-Thinking-2507            | 2025-07-25   | N/A           | N/A            | 0.811 | N/A   | 0.844    | N/A   | N/A       | N/A   | N/A           |
| QwQ-32B-Preview                          | 2024-11-28   | N/A           | N/A            | 0.652 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.500         |
| Qwen3-Next-80B-A3B-Thinking              | 2025-09-10   | N/A           | N/A            | 0.772 | N/A   | 0.827    | N/A   | N/A       | N/A   | N/A           |
| Qwen2-VL-72B-Instruct                    | 2024-08-29   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Qwen3 32B                                | 2025-04-29   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | 0.657         |
| Qwen2.5 72B Instruct                     | 2024-09-19   | N/A           | N/A            | 0.490 | N/A   | 0.711    | 0.831 | 0.866     | N/A   | 0.555         |
| Qwen3 30B A3B                            | 2025-04-29   | N/A           | N/A            | 0.658 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.626         |
| Qwen2.5 VL 7B Instruct                   | 2025-01-26   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | 0.586 | N/A           |
| Qwen3-Next-80B-A3B-Base                  | 2025-09-10   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| QvQ-72B-Preview                          | 2024-12-25   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | 0.703 | N/A           |
| Qwen2.5-Omni-7B                          | 2025-03-27   | N/A           | N/A            | 0.308 | N/A   | 0.470    | 0.715 | 0.787     | 0.592 | N/A           |
| Qwen2.5 7B Instruct                      | 2024-09-19   | N/A           | N/A            | 0.364 | N/A   | 0.563    | 0.755 | 0.848     | N/A   | 0.287         |
| Qwen3-Next-80B-A3B-Instruct              | 2025-09-10   | N/A           | N/A            | 0.729 | N/A   | 0.806    | N/A   | N/A       | N/A   | N/A           |
| Qwen2.5 VL 72B Instruct                  | 2025-01-26   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | 0.702 | N/A           |
| DeepSeek-R1-0528                         | 2025-05-28   | N/A           | N/A            | N/A   | N/A   | 0.850    | N/A   | N/A       | N/A   | 0.733         |
| DeepSeek VL2                             | 2024-12-13   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | 0.511 | N/A           |
| DeepSeek VL2 Tiny                        | 2024-12-13   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | 0.407 | N/A           |
| DeepSeek R1 Zero                         | 2025-01-20   | N/A           | N/A            | 0.733 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.500         |
| DeepSeek VL2 Small                       | 2024-12-13   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | 0.480 | N/A           |
| DeepSeek R1 Distill Qwen 7B              | 2025-01-20   | N/A           | N/A            | 0.491 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.376         |
| DeepSeek R1 Distill Qwen 1.5B            | 2025-01-20   | N/A           | N/A            | 0.338 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.169         |
| DeepSeek-R1                              | 2025-01-20   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| DeepSeek R1 Distill Llama 8B             | 2025-01-20   | N/A           | N/A            | 0.490 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.396         |
| DeepSeek R1 Distill Llama 70B            | 2025-01-20   | N/A           | N/A            | 0.652 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.575         |
| DeepSeek R1 Distill Qwen 14B             | 2025-01-20   | N/A           | N/A            | 0.591 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.531         |
| DeepSeek R1 Distill Qwen 32B             | 2025-01-20   | N/A           | N/A            | 0.621 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.572         |
| DeepSeek-V3.1                            | 2025-01-10   | N/A           | N/A            | N/A   | N/A   | 0.837    | N/A   | N/A       | N/A   | 0.564         |
| DeepSeek-V3.2-Exp                        | 2025-09-29   | N/A           | N/A            | N/A   | N/A   | 0.850    | N/A   | N/A       | N/A   | 0.741         |
| DeepSeek-V3 0324                         | 2025-03-25   | N/A           | N/A            | 0.684 | N/A   | 0.812    | N/A   | N/A       | N/A   | 0.492         |
| Grok-3 Mini                              | 2025-02-17   | N/A           | N/A            | 0.840 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.804         |
| Grok-4 Heavy                             | 2025-07-09   | N/A           | N/A            | 0.884 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.794         |
| Grok-4                                   | 2025-07-09   | N/A           | N/A            | 0.875 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.790         |
| Grok-3                                   | 2025-02-17   | N/A           | N/A            | 0.846 | N/A   | N/A      | N/A   | N/A       | 0.780 | 0.794         |
| Grok-1.5V                                | 2024-04-12   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | 0.536 | N/A           |
| GLM-4.5V                                 | 2025-08-11   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| GLM-4.5-Air                              | 2025-07-28   | N/A           | N/A            | 0.750 | N/A   | 0.814    | N/A   | N/A       | N/A   | 0.707         |
| GLM-4.5                                  | 2025-07-28   | N/A           | N/A            | 0.791 | N/A   | 0.846    | N/A   | N/A       | N/A   | 0.729         |
| Llama-3.3 Nemotron Super 49B v1          | 2025-03-18   | N/A           | N/A            | 0.667 | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Llama 3.1 Nemotron Nano 8B V1            | 2025-03-18   | N/A           | N/A            | 0.541 | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Llama 3.1 Nemotron Ultra 253B v1         | 2025-04-07   | N/A           | N/A            | 0.760 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.663         |
| Claude Opus 4.1                          | 2025-08-05   | N/A           | N/A            | 0.809 | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Claude Sonnet 4.5                        | 2025-09-29   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Claude 3.5 Haiku                         | 2024-10-22   | N/A           | N/A            | 0.416 | N/A   | 0.650    | 0.694 | 0.881     | N/A   | N/A           |
| Claude 3.7 Sonnet                        | 2025-02-24   | N/A           | N/A            | 0.848 | N/A   | N/A      | N/A   | N/A       | 0.750 | N/A           |
| Claude Sonnet 4                          | 2025-05-22   | N/A           | N/A            | 0.754 | N/A   | N/A      | N/A   | N/A       | 0.744 | N/A           |
| Claude Opus 4                            | 2025-05-22   | N/A           | N/A            | 0.796 | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Magistral Small 2506                     | 2025-06-10   | N/A           | N/A            | 0.682 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.513         |
| Magistral Medium                         | 2025-06-10   | N/A           | N/A            | 0.708 | N/A   | N/A      | N/A   | N/A       | N/A   | 0.503         |
| Devstral Medium                          | 2025-07-10   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Pixtral Large                            | 2024-11-18   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | 0.640 | N/A           |
| Mistral Small 3 24B Instruct             | 2025-01-30   | N/A           | N/A            | 0.453 | N/A   | 0.663    | 0.706 | 0.848     | N/A   | N/A           |
| Devstral Small 1.1                       | 2025-07-11   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| Codestral-22B                            | 2024-05-29   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | 0.811     | N/A   | N/A           |
| Mistral Small                            | 2024-09-17   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| GPT OSS 120B                             | 2025-08-05   | N/A           | N/A            | 0.801 | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| o3                                       | 2025-04-16   | N/A           | N/A            | 0.833 | N/A   | N/A      | N/A   | N/A       | 0.829 | N/A           |
| GPT OSS 20B                              | 2025-08-05   | N/A           | N/A            | 0.715 | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| o4-mini                                  | 2025-04-16   | N/A           | N/A            | 0.814 | N/A   | N/A      | N/A   | N/A       | 0.816 | N/A           |
| o3-pro                                   | 2025-06-10   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| o1-pro                                   | 2024-12-17   | N/A           | N/A            | 0.790 | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| GPT-5 nano                               | 2025-08-07   | N/A           | N/A            | 0.712 | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| GPT-5 mini                               | 2025-08-07   | N/A           | N/A            | 0.823 | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |
| GPT-5 Codex                              | 2025-09-15   | N/A           | N/A            | N/A   | N/A   | N/A      | N/A   | N/A       | N/A   | N/A           |

<div align="center">
Built with 💙 by the AI community, for the AI community.<br>
Star this repo if you find it useful!
</div>
