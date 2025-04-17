# 🚀 Agent Starter Pack

![Version](https://img.shields.io/pypi/v/agent-starter-pack?color=blue) [![1-Minute Video Overview](https://img.shields.io/badge/1--Minute%20Overview-gray)](https://youtu.be/jHt-ZVD660g) [![Docs](https://img.shields.io/badge/Documentation-gray)](./docs/README.md) <a href="https://studio.firebase.google.com/new?template=https%3A%2F%2Fgithub.com%2FGoogleCloudPlatform%2Fagent-starter-pack%2Ftree%2Ffeat-add-firebase-studio-resources%2Fsrc%2Fresources%2Fidx">
  <picture>
    <source
      media="(prefers-color-scheme: dark)"
      srcset="https://cdn.firebasestudio.dev/btn/try_light_20.svg">
    <source
      media="(prefers-color-scheme: light)"
      srcset="https://cdn.firebasestudio.dev/btn/try_dark_20.svg">
    <img
      height="20"
      alt="Try in Firebase Studio"
      src="https://cdn.firebasestudio.dev/btn/try_blue_20.svg">
  </picture>
</a> ![Stars](https://img.shields.io/github/stars/GoogleCloudPlatform/agent-starter-pack?color=yellow)


The `agent-starter-pack` is a collection of production-ready Generative AI Agent templates built for Google Cloud. <br>
It accelerates development by providing a holistic, production-ready solution, addressing common challenges (Deployment & Operations, Evaluation, Customization, Observability) in building and deploying GenAI agents.

| ⚡️ Launch | 🧪 Experiment  | ✅ Deploy | 🛠️ Customize |
|---|---|---|---|
| [Pre-built agent templates](./agents/) (ReAct, RAG, multi-agent, Live Multimodal API). | [Vertex AI evaluation](https://cloud.google.com/vertex-ai/generative-ai/docs/models/evaluation-overview) and an interactive playground. | Production-ready infra with [monitoring, observability](./docs/observability.md), and [CI/CD](./docs/deployment.md) on [Cloud Run](https://cloud.google.com/run) or [Agent Engine](https://cloud.google.com/vertex-ai/generative-ai/docs/agent-engine/overview). | Extend and customize templates according to your needs. |

---
 
## ⚡ Get Started in 1 Minute

Ready to build your AI agent? Simply run this command:

```bash
# Create and activate a Python virtual environment
python -m venv venv && source venv/bin/activate

# Install the agent starter pack
pip install agent-starter-pack

# Create a new agent project
agent-starter-pack create my-awesome-agent
```

**That's it!** You now have a fully functional agent project—complete with backend, frontend, and deployment infrastructure—ready for you to explore and customize.
For more installation options, see the [Installation Guide](docs/installation.md).  You can also [try it in Firebase Studio](https://studio.firebase.google.com/new?template=https%3A%2F%2Fgithub.com%2FGoogleCloudPlatform%2Fagent-starter-pack%2Ftree%2Fmain%2Fsrc%2Fresources%2Fidx) with zero setup.

---

 🆕 The starter pack offers full support for Agent Engine, a new fully managed solution to deploy agents. Simply run this command to get started:

```bash
agent-starter-pack create my-agent -d agent_engine -a adk_base
```

*See the [full list of options](docs/cli/create.md) for details.*

## 🤖 Agents

| Agent Name                  | Description                                                                                                                       |
|-----------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| `adk_base`      | A base ReAct agent implemented using Google's [Agent Development Kit](https://github.com/google/adk-python) |
| `agentic_rag` | A RAG agent for document retrieval and Q&A. Supporting [Vertex AI Search](https://cloud.google.com/generative-ai-app-builder/docs/enterprise-search-introduction) and [Vector Search](https://cloud.google.com/vertex-ai/docs/vector-search/overview).       |
| `langgraph_base_react`      | An agent implementing a base ReAct agent using LangGraph |
| `crewai_coding_crew`       | A multi-agent system implemented with CrewAI created to support coding activities       |
| `live_api`       | A real-time multimodal RAG agent powered by Gemini, supporting audio/video/text chat with vector DB-backed responses                       |

**More agents are on the way!** We are continuously expanding our [agent library](./agents/).  Have a specific agent type in mind?  [Contribute!](#contributing)

**🔍 ADK Samples**

Looking to explore more ADK examples? Check out the [ADK Samples Repository](https://github.com/google/adk-samples) for additional examples and use cases demonstrating ADK's capabilities.

#### Extra Features

The `agent-starter-pack` offers two key features to accelerate and simplify the development of your agent:

- **🔄 [CI/CD Automation (Experimental)](docs/cli/setup_cicd.md)** - One command to set up a complete GitHub + Cloud Build pipeline for all environments
- **📥 [Data Pipeline for RAG with Terraform/CI-CD](docs/data-ingestion.md)** - Seamlessly integrate a data pipeline to process embeddings for RAG into your agent system. Supporting [Vertex AI Search](https://cloud.google.com/generative-ai-app-builder/docs/enterprise-search-introduction) and [Vector Search](https://cloud.google.com/vertex-ai/docs/vector-search/overview).


## High-Level Architecture

This starter pack covers all aspects of Agent development, from prototyping and evaluation to deployment and monitoring.

![High Level Architecture](docs/images/ags_high_level_architecture.png "Architecture")

---

## 🔧 Requirements

- Python 3.10+
- [Google Cloud SDK](https://cloud.google.com/sdk/docs/install)
- [Terraform](https://developer.hashicorp.com/terraform/downloads) (for deployment)


## 📚 Documentation
See the [documentation](docs/) for more details:

- [Why Use the Starter Pack?](docs/why_starter_pack.md)
- [Installation](docs/installation.md)
- [Deployment](docs/deployment.md)
- [Data Ingestion](docs/data-ingestion.md)
- [Observability](docs/observability.md)
- [CLI Reference](docs/cli/README.md)
- [Troubleshooting](docs/troubleshooting.md)

### Video Walkthrough:

- **March 6, 2025**: A [120 Minute livestream video demo](https://www.youtube.com/watch?v=yIRIT_EtALs&t=235s) of the new `agent-starter-pack` were we build 3 Agents under 30 minutes!
- **Oct 29, 2024**: A [20-Minute Video Walkthrough](https://youtu.be/kwRG7cnqSu0) is available, showcasing the previous `agent-starter-pack`.

## Explore More Generative AI Resources

Looking for more examples and resources for Generative AI on Google Cloud? Check out the [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai) repository for notebooks, code samples, and more!

## Contributing

Contributions are welcome! See the [Contributing Guide](CONTRIBUTING.md).

## Feedback

We value your input! Your feedback helps us improve this starter pack and make it more useful for the community.

### Getting Help

If you encounter any issues or have specific suggestions, please first consider [raising an issue](https://github.com/GoogleCloudPlatform/generative-ai/issues) on our GitHub repository.

### Share Your Experience

For other types of feedback, or if you'd like to share a positive experience or success story using this starter pack, we'd love to hear from you! You can reach out to us at <a href="mailto:agent-starter-pack@google.com">agent-starter-pack@google.com</a>.

Thank you for your contributions!

## Disclaimer

This repository is for demonstrative purposes only and is not an officially supported Google product.

## Terms of Service

The agent-starter-pack templating CLI and the templates in this starter pack leverage Google Cloud APIs. When you use this starter pack, you'll be deploying resources in your own Google Cloud project and will be responsible for those resources. Please review the [Google Cloud Service Terms](https://cloud.google.com/terms/service-terms) for details on the terms of service associated with these APIs.
