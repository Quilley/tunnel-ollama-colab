# Hosting Ollama on Colab Servers

This project provides a Colab notebook to install and host Ollama on a Colab server, making it accessible over the internet using ngrok.

## Steps

1. **Install Ollama**
   - The notebook downloads and installs Ollama using a shell script.

2. **Install Dependencies**
   - Installs `aiohttp` and `pyngrok` Python packages for networking and tunneling.

3. **Set Up Environment**
   - Sets the `LD_LIBRARY_PATH` for NVIDIA libraries (required for GPU support).

4. **Configure ngrok**
   - You must register at [ngrok.com](https://ngrok.com/) and obtain an authtoken.
   - Replace `api-token` in the notebook with your actual ngrok authtoken.

5. **Run Ollama and Expose via ngrok**
   - The notebook starts the Ollama server and exposes it to the internet using ngrok.
   - The public ngrok URL will be shown in the output.

## Usage

- Open the notebook in Google Colab.
- Follow the instructions in each cell.
- Make sure to replace the ngrok authtoken placeholder with your own.

## Notes

- This setup is for demonstration and testing purposes.
- Do not expose sensitive or production workloads using this method.
