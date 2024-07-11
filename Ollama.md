# Amazing New VS Code AI Coding Assistant with Open Source Models

src = https://www.youtube.com/watch?v=he0_W5iCv-I

---

## Intro

- a free AI coding assistant that we can use in VS Code
- it allows us to keep our code 100% local
- uses free open source models that are capable of giving us as good or even better results than we might be getting from a Copilot subscription

---

## Install Ollama

- start at https://ollama.com/
- download ollama for your OS and install it
- this might be helpful for Arch users: https://www.jeremymorgan.com/blog/generative-ai/how-to-install-ollama-web-ui-arch-linux/
- once you've installed ollama, start VS Code and open a terminal window
- run `ollama --version` to make sure it's been installed and is recognized by your system
- if this cmd is not recognized, reboot

---

## Add an Open Source Model / LLM (large language model)

- go to this page: https://evalplus.github.io/leaderboard.html
- this page is comparing free and paid models
- select your free model and go back to https://ollama.com/ to search for this model
- copy the command that will install the model: `ollama run <model_name>`
- paste it in your terminal window in VS Code, and run it
- downloading the model can take time depending on your connection and the model size

---

## Continue for VS Code

- now that you've installed Ollama and the desired free model, you need to add the ***Continue*** extension to VS code
- https://www.continue.dev/
- in VS code, go to the Extensions menu and search for "continue"
- install the extension

>[!tip]
>when opening Continue, you might get recommendations on the splash screen, just skip them, we don't want the splash screen

- a Continue icon will appear in the left pane, click it
- click on the gear icon to configure Continue
- inside this config.json file, you can see:
  - the available models
    - the default model is listed at the top
  - the custom commands
    - for ex, if we type "test" into the chat, it will run the specified prompt against the current AI model
  - then you can specify the desired tabAutocompleteModel

### Custom command example

- select the existing custom command and press Shift+Ctrl+Alt + the down arrow to copy-paste it
- put a comma after the first custom command (after the closing curly bracket)
- in this new custom command:
  - set the "name" value to "step"
  - set the "prompt" value to "explain the selected code step by step"
  - set the "description" value to "code explanation"
- now you can write some code and try your new custom command in the chat window

---

## Code Chats & Autocompletions

### AI-Generated Code 

- we can create a .js file named "convertToMySQLTimestamp.js"
- after that we can press Ctrl + I to 



@6/10
