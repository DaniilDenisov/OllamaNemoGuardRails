# OllamaNemoGuardRails
## Sample code for Nemo Guardrails with Local Ollama
Original OpenAI-based tutorial is here:
https://docs.nvidia.com/nemo/guardrails/latest/getting-started/4-input-rails/README.html

**config** folder contains `config.yml` and `prompts.yml` both files needed for running Nemo Guardrails application.

**You may run this app in interactive mode:**
CD into venv folder (where you store the source) C:\Users\user\Desktop\PythonVenv\NeMoGuardRails> and run guardrails interactive session with:
`nemoguardrails chat --config=config`
This will allow you ask the model what you want.

**And you may run this as usual python script (with active venv):**
`python Sample.py`
This will run two prompts - one jailbreak attempt and good one.

The requirements.txt contain only the pip packages (nemoguardrails, langchain-ollama, colorama). No models.

To fuction properly you should install ollama (https://ollama.com/download) and pull and serve llama3 model (https://ollama.com/library/llama3.1:8b):
`ollama run llama3.1:8b`
