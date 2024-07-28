# Ollama and Ngrok in Google Colab

![image](https://github.com/user-attachments/assets/083c9803-5b12-4cae-b7c6-3f13b9e1c5ab)


This repository demonstrates how to set up and run Ollama with Ngrok in a Google Colab environment.

## Steps

1. **Install Ollama:** The notebook uses a shell script from the official Ollama website to install Ollama.
2. **Install Ngrok:** It utilizes `pip` to install the `pyngrok` library.
3. **Run Ollama and Expose with Ngrok:**
    * Set your Ngrok authentication `token`.
    * Define an asynchronous function to run processes (Ollama and Ngrok).
    * Start Ollama using the `ollama serve` command.
    * Expose Ollama using Ngrok on port 11434.
4. **Add Ollama Host venv (macos):**
   ```
   export OLLAMA_HOST=url
   ```
5. Test:
   ```
   ollama run model_name
   ```


## Local Installation

**Ollama:**

1. Download the Ollama
```
https://ollama.com/download
```

**Ngrok:**

Sign up for an Ngrok account and get your authtoken.
   ```
   https://dashboard.ngrok.com/get-started/your-authtoken
   ```

## Note
* Ollama Host venv for other OS:
```
  https://github.com/ollama/ollama/blob/main/docs/faq.md
```

* Remember to replace `AUTH_TOKEN` with your actual Ngrok authentication token.
* This setup allows you to access your Ollama instance remotely through the Ngrok tunnel.
