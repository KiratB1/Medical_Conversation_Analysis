# Medical Conversation Analysis Tool

## Automated Transcription, Classification, and Summarization for Healthcare Professionals

This project provides a comprehensive suite of tools for processing and analyzing medical conversations between doctors and patients. It leverages cutting-edge natural language processing techniques to transcribe audio, classify speaker roles, and generate concise summaries.

## Dataset used and referenced: 
A dataset of simulated patient-physician medical interviews with a focus on respiratory cases was used to create visualizations in this repository 
(https://www.nature.com/articles/s41597-022-01423-1)

### Key Features

1.  **Audio Transcription**  
  Converts `.mp3` audio files to text using [AssemblyAI's API](https://www.assemblyai.com/).
2. **Speaker Classification**: Implements both AI-powered and rule-based approaches to distinguish between doctor and patient speech.
3. **Conversation Summarization**: Employs advanced transformer models to create concise summaries of medical dialogues.
4. **Medical Named Entity Recognition**: Integrates with Hugging Face's Medical-NER model for identifying medical terms and concepts.
5.  **SOAP Note Summarization**  
  Uses OpenAI's GPT model (zero-shot) to generate structured SOAP notes:  
  **S**ubjective, **O**bjective, **A**ssessment, **P**lan.

6. **Disease and Symptom Extraction**  
  Extracts illnesses and symptoms mentioned in transcripts using GPT-based zero-shot classification.

7. **Medical Category Classification**  
  Groups each conversation by major body systems (e.g., respiratory, cardiac) based on symptoms detected.

8. **Visualization**  
  Generates pie charts of disease distribution and calculates RMSE when compared to expert-labeled data from the original [SEMI dataset](https://www.nature.com/articles/s41597-022-01423-1).



### Use Cases

- Streamline medical documentation processes
- Enhance patient record accuracy and completeness
- Support medical research and analysis
- Improve healthcare provider training and education

### Getting Started

1. Clone the repository
2. Install required dependencies
3. Set up API keys for OpenAI services
4. Run the main script to process your medical conversations

### Results
- AI classifications were compared to expert-labeled categories from the SEMI dataset.

- RMSE (Root Mean Square Error) between AI-classified and ground truth diagnosis categories: 7.74%

- Most discrepancies were in the respiratory, cardiac, and gastrointestinal categories, likely due to zero-shot GPT classification not matching expert manual labels.
### Technologies Used

- Python
- OpenAI
- assemblyAI


Enhance your medical practice with our state-of-the-art conversation analysis tool. Improve patient care, streamline documentation, and gain valuable insights from doctor-patient interactions.
