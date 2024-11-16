# open-webui

![msedge_RPjqBl8yNq](https://github.com/user-attachments/assets/e153e64b-4c05-4fbb-8315-9604817679f4)

Run Open WebUI seamlessly using the OpenAI API or llama models.

| [:sparkles: Getting Started](#getting-started) | [:rocket: Quick Setup](#quick-setup) |
| ----------------- | ----------- |

## Getting Started
Follow these steps to set up and run Open WebUI with OpenAI's API:
1. [Ensure you meet all requirements](#requirements).
2. [Clone the repository and configure](#clone-and-configure).
3. Start the service effortlessly using Docker Compose.

## Requirements
Before starting, ensure you have the following installed:
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- OpenAI API key. (Sign up at [OpenAI](https://platform.openai.com/api-keys) to obtain one.)

## Quick Setup
### Clone and Configure
1. Clone the repository:
   ```bash
   git clone https://github.com/germanfica/open-webui-docker.git open-webui
   cd open-webui
   ```
2. Ensure your OpenAI API key is correctly set in the environment configuration. You have two options:
   - __Option 1: Use a `.env` file__

      Create a .env file and add your API key:
      ```env
      OPENAI_API_KEY=your_openai_api_key_here
      ```
   - __Option 2: Export the API key directly__

      If you prefer not to use a `.env` file, you can export the API key directly to your operating system's environment variables:

      __Export in PowerShell:__
      ```powershell
         setx OPENAI_API_KEY "your_api_key_here"
      ```

      __Export on macOS or Linux:__
      ```
         export OPENAI_API_KEY="your_api_key_here"
      ```

      Make sure to replace `your_api_key_here` with the actual API key obtained from the OpenAI dashboard. For detailed instructions on creating and exporting an API key, refer to the [OpenAI Quickstart Guide](https://platform.openai.com/docs/quickstart#create-and-export-an-api-key).

## Start the Service

Run the following command to start the Open WebUI using OpenAI's API:

```bash
docker compose -f docker-compose.openai.yml up -d
```

This will pull the necessary images and start the containerized application.

## Access the WebUI

Once the container is up, you can access the Open WebUI through your browser at http://localhost:3010 (or the port you have configured in docker-compose.openai.yml).

## Credits
- [German Fica](https://germanfica.com/)

## External tools
OpenAI API for providing backend intelligence.

## License
[MIT](https://opensource.org/licenses/MIT)
