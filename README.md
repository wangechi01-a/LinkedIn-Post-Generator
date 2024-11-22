# LinkedIn Post Pro

## Overview

**LinkedIn Post Pro** is a Python-based application designed to help users generate engaging and dynamic LinkedIn posts for various professional topics. The app leverages natural language processing (NLP) to automatically generate posts in both English and Swahili. Whether you're a professional, content creator, or a business looking to engage your audience, LinkedIn Post Pro can help create posts tailored to your needs.

## Features

- **Multi-language Support**: Automatically generates LinkedIn posts in both English and Swahili.
- **Customizable Content**: Input your professional topic or keyword, and the app will generate a relevant and engaging post.
- **Ease of Use**: A simple and user-friendly interface makes it easy to generate posts with minimal effort.
- **Dynamic Content Generation**: Generates posts based on your chosen tags or topics to help you engage with your audience effectively.
- **Optimized for LinkedIn**: Posts are crafted with LinkedIn’s audience in mind, ensuring relevance and engagement.

## Requirements

- **Python 3.x**
- **Libraries/Packages**:
  - `transformers`
  - `langchain`
  - `pandas`
  - `openai` (for GPT-based generation)
  - `streamlit` (for UI)
  - `pyyaml`
  - **Others**: Refer to `requirements.txt` for full list of dependencies.

## Installation

### Step 1: Clone the repository

```bash
git clone https://github.com/yourusername/linkedin-post-pro.git
```

### Step 2: Install dependencies

Navigate to the project directory and install the necessary dependencies using pip:

```bash
cd linkedin-post-pro
pip install -r requirements.txt
```

### Step 3: Set up environment variables

Create a `.env` file in the project root and add the following variables:

```
OPENAI_API_KEY=your_openai_api_key
```

### Step 4: Run the application

You can run the app using the following command:

```bash
streamlit run app.py
```

This will launch the LinkedIn Post Pro app on your local machine. Follow the instructions on the web interface to start generating LinkedIn posts.

## How to Use

1. **Enter the Topic**: In the provided input box, type in the topic you want your post to focus on (e.g., AI, Data Science, Career Growth, etc.).
2. **Generate the Post**: Click the "Generate" button, and the app will create a post based on your topic. You will receive a generated post in both English and Swahili.
3. **Post to LinkedIn**: Copy and paste the generated post into your LinkedIn feed and share with your network!

## Project Structure

Here is the directory structure of the project:

```
linkedin-post-pro/
│
├── app.py                     # Main application file that runs the Streamlit app
├── requirements.txt            # List of required Python packages
├── .env                        # Environment variables for API keys (like OpenAI API key)
├── README.md                   # Project documentation (this file)
├── config.py                   # Configuration file for application settings
├── utils.py                    # Utility functions for generating posts
├── posts_generator/            # Folder for all logic related to generating posts
│   ├── english_generator.py    # Logic for generating posts in English
│   └── swahili_generator.py    # Logic for generating posts in Swahili
└── assets/                     # Folder for images, icons, and other static assets
    └── logo.png                # App logo or related graphics
```

### Key Files

- `app.py`: This file runs the Streamlit app and provides the user interface for generating LinkedIn posts.
- `requirements.txt`: A list of Python dependencies required for the application to work.
- `.env`: Stores sensitive information like API keys (e.g., OpenAI API key).
- `config.py`: Contains configurations for setting up API keys and other app-specific settings.
- `utils.py`: Contains helper functions used in generating the posts.
- `posts_generator/`: Directory containing the logic for generating posts in both English and Swahili.
- `assets/`: Stores image files and other static resources used by the app.

## Example Usage

```python
# Example to generate posts on Career Growth
app.generate_post("Career Growth")
```

This will generate posts related to career development, tips, and growth strategies.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

