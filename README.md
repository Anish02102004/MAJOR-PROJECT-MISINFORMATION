# MAJOR-PROJECT-MISINFORMATION

## Project Overview
This project is a Flask-based web application for detecting dementia-related misinformation. It combines a fine-tuned DistilBERT classifier, dataset-driven training files, and a web research agent to help assess whether a claim is likely to be trustworthy or misleading.

The app is designed to support research and fact-checking around dementia-related claims by comparing text against learned patterns, reference datasets, and evidence gathered from web research sources.

## Key Features
- Web interface built with Flask and HTML templates.
- Dementia misinformation detection using a fine-tuned transformer model.
- Support for evidence-assisted checking through a web research agent.
- Dataset files for training, testing, and evaluation.
- Basic performance and reporting utilities for research workflows.

## How It Works
1. A user submits a claim or text through the web app.
2. The model analyzes the text and predicts whether it looks like misinformation.
3. The research layer can gather supporting evidence from medical and web sources.
4. The app returns a result that can be used for review or fact-checking.

## Project Structure
- `app.py` - Main Flask application.
- `web_research_agent.py` - Web research and evidence lookup helpers.
- `config.py` - Configuration values and API key placeholders.
- `templates/index.html` - Front-end page for the app.
- `train_dataset.csv` - Training data.
- `test_dataset.csv` - Test data.
- `dementia_misinformation_dataset_500.csv` - Core dataset used by the project.
- `Fine_tune.py` - Model fine-tuning script.

## Setup
1. Install Python dependencies:

```bash
pip install -r requirements.txt
```

2. Run the application:

```bash
python app.py
```

3. Open the local Flask URL shown in the terminal.

## Notes
- Large files such as PDFs and temporary files are ignored from version control.
- API credentials should be kept out of the README and managed in configuration or environment variables.

