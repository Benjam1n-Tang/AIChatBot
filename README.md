# AIChatBot

A simple AI chatbot built with Python that uses OpenAI's GPT-4.1 model through GitHub's marketplace integration.

## Features

- Interactive command-line chatbot interface
- Powered by OpenAI GPT-4.1 model
- Environment variable configuration for secure token management
- Easy dependency management with pipenv

## Prerequisites

- Python 3.7 or higher
- pipenv (for dependency management)
- GitHub account with access to OpenAI models

## Installation

1. Clone this repository:
```bash
git clone <your-repository-url>
cd AIChatBot
```

2. Install dependencies using pipenv:
```bash
pipenv install
```

3. Activate the virtual environment:
```bash
pipenv shell
```

## Configuration

1. Get your GitHub token for OpenAI model access:
   - Visit: https://github.com/marketplace/models
   - Follow the instructions to obtain your token

2. Create a `.env` file in the project root directory:
```bash
touch .env
```

3. Add your GitHub token to the `.env` file:
```
GITHUB_TOKEN=your_github_token_here
```

**Important:** Never commit your `.env` file to version control. Make sure it's included in your `.gitignore` file.

## Usage

Run the chatbot:
```bash
python main.py
```

The chatbot will start and you can begin interacting with it through the command line interface.

## Dependencies

This project uses the following Python packages:

- `openai` - OpenAI API client library
- `python-dotenv` - Load environment variables from .env files
- `os` - Built-in Python module for operating system interface

All dependencies are managed through `Pipfile` and can be installed with `pipenv install`.

## Project Structure

```
AIChatBot/
├── main.py          # Main application file
├── .env             # Environment variables (create this file)
├── Pipfile          # Pipenv dependencies
├── Pipfile.lock     # Locked dependency versions
└── README.md        # This file
```

## Security Notes

- Keep your GitHub token secure and never share it publicly
- The `.env` file contains sensitive information and should not be committed to version control
- Add `.env` to your `.gitignore` file to prevent accidental commits

## Troubleshooting

- **Token Issues**: Make sure your GitHub token is valid and has the necessary permissions for OpenAI model access
- **Import Errors**: Ensure you're running the script within the pipenv virtual environment (`pipenv shell`)
- **API Errors**: Check that your token is correctly set in the `.env` file with the exact format: `GITHUB_TOKEN=your_token`

## Contributing

Feel free to submit issues, fork the repository, and create pull requests for any improvements.

## Author

Benjamin Tang  
GitHub: [Benjam1n-Tang](https://github.com/Benjam1n-Tang)  
LinkedIn: [BTang22](https://linkedin.com/in/BTang22)
