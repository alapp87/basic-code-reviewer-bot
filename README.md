# Code Reviewer

This repository contains a Python script that utilizes the OpenAI GPT-3.5 language model to generate code reviews for files. The script analyzes the content of a given file and provides suggestions for improving its style, performance, readability, and maintainability. It also recommends the introduction of reputable libraries to enhance the code quality. The generated code review aims to be both constructive and helpful.

## Prerequisites

Before using the script, make sure you have the following:

- Python: You need to have Python installed on your system. If not, you can download and install it from the [Python website](https://www.python.org/downloads/).

- OpenAI API Key: To use the OpenAI GPT-3.5 model, you need an API key from OpenAI. If you don't have one, sign up on the [OpenAI website](https://beta.openai.com/signup/) and obtain your API key.

## Installation

1. Install the required Python packages using pip.

   ```bash
   pip install -r requirements.txt
   ```

2. Create a `.env` file in the same directory as the script and add your OpenAI API key.

   ```env
   OPENAI_API_KEY=your-api-key-here
   ```

## Usage

Run the script with the following command:

```bash
python code_reviewer.py file_to_review.py
```

Replace `file_to_review.py` with the path to the file you want to analyze.

### Optional Arguments

- `--model`: Specifies the GPT-3.5 model variant to use. The default is `"gpt-3.5-turbo"`.

## How It Works

The script reads the content of the input file and sends a conversation to the GPT-3.5 model. The conversation includes a system prompt describing the task and a user message containing the content of the file to be reviewed. The model then generates suggestions for improvements, including changes to style, performance, readability, and maintainability. The script displays the model's suggestions in the console.

## Notes

- The generated code reviews are based on the patterns and information available in the training data of the GPT-3.5 model. The suggestions provided by the model might not always be perfect or entirely accurate.

- The script utilizes the OpenAI Python library to interact with the API. Make sure to keep your API key secure and do not share it publicly.

- Feel free to modify the script according to your needs, such as integrating it into a larger project or customizing the review criteria.

## License

This project is licensed under the [MIT License](LICENSE).

---

Please feel free to contribute to the repository, report any issues, or suggest improvements. Your feedback is valuable!
