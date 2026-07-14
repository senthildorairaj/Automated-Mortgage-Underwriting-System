# Senior-Mortgage-Underwriting-System
Comprehensive agentic AI system for mortgage underwriting that automates credit analysis, income verification, asset assessment, and collateral evaluation while maintaining compliance with Fair Lending regulations and implementing human oversight for high-risk decisions.
# Senior Mortgage Underwriting System

## Project Overview

This project implements an **Agentic AI Multi-Agent Workflow** for a Senior Mortgage Underwriting System. It demonstrates how to build an intelligent loan analysis system using LangGraph and AI agents to automate and streamline the mortgage underwriting process.

Traditional mortgage underwriting is often time-consuming, document-heavy, inconsistent, and expensive. This AI-powered system addresses these challenges by:

- **Reducing processing time** from days to hours.
- Maintaining **consistent decision quality**.
- Providing an **audit trail** with clear reasoning chains.
- Ensuring **regulatory compliance** (e.g., Fair Lending Act).
- Scaling to handle **thousands of applications** simultaneously.

## Learning Objectives

By exploring this project, you will be able to:

- **Understand Multi-Agent Systems**: Learn how specialized AI agents collaborate to solve complex problems.
- **Implement Agent Workflows**: Build coordinated workflows using LangGraph's state machine architecture.
- **Apply RAG Patterns**: Integrate retrieval-augmented generation for policy compliance.
- **Handle PII & Compliance**: Implement data sanitization and bias detection mechanisms.
- **Create HITL Systems**: Design human-in-the-loop workflows for high-risk decisions.
- **Production Deployment**: Understand real-world deployment considerations and monitoring.

## System Architecture

The system utilizes a hierarchical multi-agent pattern with Specialist Agents (Credit, Income, Asset, Collateral Analysts) and Coordination Agents (Supervisor, Critic, Decision Agents). 


## Technology Stack

- **LangGraph**: Agent orchestration & state management
- **LangChain**: LLM integration & tool management
- **OpenAI - GPT-4o-mini**: Language model for reasoning
- **ChromaDB**: Vector store for policy retrieval
- **Python**: Programming language

## Setup and Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-repo/your-project.git
    cd your-project
    ```

2.  **Install dependencies:**
    ```bash
    pip install \
      langgraph==1.0.5 \
      langchain==1.0.0 \
      langchain-openai==1.1.7 \
      langchain-community==0.4.1 \
      langchain-text-splitters==1.1.0 \
      chromadb==1.4.0 \
      pypdf==6.6.0
    ```

3.  **API Configuration:**
    This project uses an OpenAI-compatible API. You will need to set your `OPENAI_API_KEY` and `OPENAI_API_BASE` as environment variables or load them from a `config.json` file. Ensure `config.json` contains:
    ```json
    {
      "API_KEY": "YOUR_API_KEY",
      "OPENAI_API_BASE": "YOUR_API_BASE_URL"
    }
    ```
    *Note: For Google Colab, you can use Colab secrets for API keys.* 

## Usage

This project is best explored in a Jupyter Notebook or Google Colab environment. The `mortgage_underwriting_system.ipynb` notebook guides you through:

- Defining data models and state management.
- Building core components like utility tools, PII sanitization, and RAG policy retrieval.
- Implementing specialist agents (Credit, Income, Asset, Collateral, Critic, Decision).
- Integrating the complete workflow using LangGraph.
- Testing and evaluating the system with various test cases.
- Understanding production deployment considerations.

To run the notebook:

1.  Open `mortgage_underwriting_system.ipynb` in your preferred environment.
2.  Execute cells sequentially to follow the multi-agent workflow development.



### Part 1: Core Agent Implementation
- Utility tools for calculations 
- PII sanitization system 
- Bias detection mechanism
- RAG policy retrieval
- Test data preparation

### Part 2: Workflow & Orchestration
- Income Analyst Agent Implementation
- Asset Analyst Agent Implementation
- Collateral Analyst Agent Implementation
- Critic Agent Implementation
- Decision Agent Implementation
- Defining state and workflow/graph correctly

### Part 3: Testing & Analysis
- Run all test cases

### Part 4: Summary and Future Scope
- Summary / Your Observations about this Project
- Future scope of this Project 

## Future Scope

- Expand into full AUS capabilities with additional agents and rule engines.
- Integrate real-time data sources and external APIs (e.g., credit bureaus, bank statements).
- Build a full UI dashboard and case management system for operational visibility.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the JHU License - see the LICENSE file for details.
