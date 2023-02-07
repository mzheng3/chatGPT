## chatGPT

This repository gives you step-by-step procedure to install ChatGPT locally on your machine. 

**Step One:** Install Python 3.7 or later via https://www.python.org

**Step Two:** Set up an API key via https://beta.openai.com/signup

**Step Three:** Install required Python libraries

Run the following commands: 

- pip install openai
- pip install requests numpy tqdm

**Step Four:** Codes for ChatGPT

Run the following commands:

- import openai
- openai.api_key = "your own openAI API key"
- model_engine = "text-davinci-003"
- prompt = "your inquiry"
- completion = openai.Completion.create(engine = model_engine, prompt = prompt, max_token = 4097, n = 1, stop = None, temperature = 0.7)
- message = completion.choices[0]['text']
- print(message)


