# Prompt Injection Defense Project

This repository contains the code and resources for a research project on prompt injection defense mechanisms in medical image analysis using Large Language Models (LLMs).

## Contents

1. `prompt_injection_defense_agent.py`: Python script for analyzing medical images using various LLM models with an agent-based approach.
2. `prompt_injection_defense_ethical.py`: Python script for analyzing medical images using various LLM models with an ethical prompt variation.
3. `R_readme.md`: Instructions for visualization using R (located in the same folder).

## Requirements

To run the analysis, you'll need:

1. Python 3.7+
2. Required Python libraries: 
   - anthropic
   - openai
   - openpyxl
   - python-dotenv
   - reka
   - pandas

3. API keys for:
   - Anthropic (Claude models)
   - OpenAI (GPT-4 models)
   - Reka (Reka-Core model)

4. Medical images: 90 images named "Folie1.jpg" to "Folie90.jpg" in a folder named "Images_Mitigation". These images can be obtained from the publication website under Extended Data for full reproducibility.

## Setup

1. Clone this repository.
2. Install required Python libraries: `pip install anthropic openai openpyxl python-dotenv reka pandas`
3. Create three `.env` files in the project root:
   - `api_claude.env`: Contains `API_KEY_CLAUDE=your_anthropic_api_key`
   - `api_gpt4.env`: Contains `OPENAI_API_KEY=your_openai_api_key`
   - `api_reka.env`: Contains `REKA_API_KEY=your_reka_api_key`
4. Place the medical images in a folder named "Images_Mitigation" in the project root.

## Usage

1. Run `prompt_injection_defense_agent.py` for the agent-based analysis:
   ```
   python prompt_injection_defense_agent.py
   ```

2. Run `prompt_injection_defense_ethical.py` for the ethical prompt variation analysis:
   ```
   python prompt_injection_defense_ethical.py
   ```

Both scripts will generate an Excel file named "Mitigation_PI_revision.xlsx" with the analysis results.

## Visualization

For visualizing the results, please refer to the `R_readme.md` file in this repository. It contains instructions on how to use R for data visualization based on the generated Excel file.

## Note

This project is part of a research study. Please ensure you have the necessary permissions and comply with ethical guidelines when working with medical images and AI models.

For any questions or issues, please open an issue in this GitHub repository.
