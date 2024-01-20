# 🤖 SeleniumTestGPT: An experimental Selenium E2E Test Generator 

SeleniumTestGPT is an AutoGPT experiment that utilizes [Langchain](https://github.com/hwchase17/langchain) and [Selenium](https://github.com/SeleniumHQ/selenium) to enable an AutoGPT agent take control of an entire Chrome session and generate end to end tests.


<h2 align="center"> Requirements </h2>

- Chrome
- Python >3.8
- Install [Poetry](https://python-poetry.org/docs/#installation)

<h2 align="center"> 🛠️ Setup </h2>

1. Set up your OpenAI [API Keys](https://platform.openai.com/account/api-keys) and add `OPENAI_API_KEY` env variable
2. Install Python requirements via poetry `poetry install`
3. Open a poetry shell `poetry shell`
4. Run chromegpt via `python -m chromegpt`

<h2 align="center"> 🧠 Usage </h2>

- GPT-3.5 Usage (Default): `python -m chromegpt -v -t "{your request}"`
- GPT-4 Usage (Recommended, needs GPT-4 access): `python -m chromegpt -v -a auto-gpt -m gpt-4 -t "{your request}"`
- For help: `python -m chromegpt --help`
```
Usage: python -m chromegpt [OPTIONS]

  Run ChromeGPT: An AutoGPT agent that interacts with Chrome

Options:
  -t, --task TEXT                 The task to execute  [required]
  -a, --agent [auto-gpt|baby-agi|zero-shot]
                                  The agent type to use
  -m, --model TEXT                The model to use
  --headless                      Run in headless mode
  -v, --verbose                   Run in verbose mode
  --human-in-loop                 Run in human-in-loop mode, only available
                                  when using auto-gpt agent
  --help                          Show this message and exit.
```

