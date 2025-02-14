# Log Classification System Using Deepseek R1 LLM, NLP, Regex, BERT

This project is a log classification system that utilizes various techniques including Regex, BERT, and LLM to classify log messages. The system is designed to handle logs from different sources and apply the appropriate classification method based on the source.

## Project Structure

```
Log Classification System Using Deepseek R1 LLM, NLP, Regex, BERT/
│
├── Dataset/
│   └── training.ipynb
├── models/
│   └── log_message_classifier.joblib
├── processor_regex.py
├── processor_llm.py
├── processor_bert.py
├── classify.py
├── .env
└── README.md
```

## Files Description

- **Dataset/training.ipynb**: Jupyter notebook for training and evaluating the classification models.
- **models/log_message_classifier.joblib**: Trained logistic regression model for classifying log messages.
- **processor_regex.py**: Contains the function `classify_with_regex` for classifying log messages using regex patterns.
- **processor_llm.py**: Contains the function `classify_with_llm` for classifying log messages using a language model.
- **processor_bert.py**: Contains the function `classify_with_bert` for classifying log messages using BERT embeddings.
- **classify.py**: Main script for classifying log messages from different sources.
- **.env**: Environment file containing API keys and other configurations.
- **README.md**: This file.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/log-classification-system.git
    cd log-classification-system
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

4. Set up the environment variables:
    ```sh
    cp .env.example .env
    # Edit the .env file to add your GROQ API key and other configurations
    ```

## Usage

### Classifying Logs

To classify logs from a CSV file, run the following command:
```sh
python classify.py
```
This will classify the logs in `test.csv` and save the results to `output.csv`.

### Training the Model

To train the model, open the `Dataset/training.ipynb` notebook and follow the instructions to train and evaluate the model.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.