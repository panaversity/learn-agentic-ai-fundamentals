# CrewAI Hello World Default Flows Template

Welcome to the Crew project, powered by [crewAI](https://crewai.com). This default template is designed to help you set up a multi-agent AI system with ease, leveraging the powerful and flexible framework provided by crewAI. Our goal is to enable your agents to collaborate effectively on complex tasks, maximizing their collective intelligence and capabilities. We have not made any changes in this default template.

[Documentation](https://docs.crewai.com/installation)

[CrewAI GPT](https://chatgpt.com/g/g-qqTuUWsBY-crewai-assistant)

## Installation

Ensure you have [Python 3.12](https://www.python.org/downloads/) installed on your system. This project uses [UV](https://docs.astral.sh/uv/) for dependency management and package handling, offering a seamless setup and execution experience.

First, if you haven't already, install uv:

```bash
pip install uv
```
Note: On Mac give pip3 commands

Now [install CrewAI](https://docs.crewai.com/installation):

```bash
pip install crewai crewai-tools
```
Verify the Installation

```bash
pip freeze | grep crewai
```

## Create Flows Project

[Read Flows Documentation](https://docs.crewai.com/concepts/flows)

```bash
crewai create flow helloworld
```
Note the name should be only text

Next, navigate to your project directory and install the dependencies:

```bash
cd helloworld
```

Lock the dependencies and install them by using the CLI command:

```bash
crewai install
```

## Add Key

**Add your `OPENAI_API_KEY=` into the `.env` file**

## Customizing

- Modify `src/helloworld/config/agents.yaml` to define your agents
- Modify `src/helloworld/config/tasks.yaml` to define your tasks
- Modify `src/helloworld/crew.py` to add your own logic, tools and specific args
- Modify `src/helloworld/main.py` to add custom inputs for your agents and tasks. Also define the flow.

## Running the Project

To kickstart your crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
crewai flow kickoff
```

This command initializes the helloworld Crew, assembling the agents and assigning them tasks as defined in your configuration.

This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.

## Understanding Your Crew

The helloworld Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.

## Support

For support, questions, or feedback regarding the Crew or crewAI.

- Visit our [documentation](https://docs.crewai.com)
- Reach out to us through our [GitHub repository](https://github.com/joaomdmoura/crewai)
- [Join our Discord](https://discord.com/invite/X4JWnZnxPb)
- [Chat with our docs](https://chatg.pt/DWjSBZn)

Let's create wonders together with the power and simplicity of crewAI.