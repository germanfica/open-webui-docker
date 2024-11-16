# open-webui

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
2. Ensure your OpenAI API key is correctly set in the environment configuration. Create a `.env` file if necessary:

   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   ```

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
