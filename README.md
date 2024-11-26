
# REACT Agent - Intelligent Task Processing System


[![Join our Discord](https://img.shields.io/badge/Discord-Join%20our%20server-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/agora-999382051935506503) [![Subscribe on YouTube](https://img.shields.io/badge/YouTube-Subscribe-red?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@kyegomez3242) [![Connect on LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kye-g-38759a207/) [![Follow on X.com](https://img.shields.io/badge/X.com-Follow-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://x.com/kyegomezb)


[![GitHub stars](https://img.shields.io/github/stars/The-Swarm-Corporation/Legal-Swarm-Template?style=social)](https://github.com/The-Swarm-Corporation/Legal-Swarm-Template)
[![Swarms Framework](https://img.shields.io/badge/Built%20with-Swarms-blue)](https://github.com/kyegomez/swarms)



A production-grade AI agent implementing the REACT (Reason + Act) methodology with YAML configuration and JSON tool interactions. Built with the Swarms framework and powered by advanced language models.

## 🌟 Features

### Intelligent Reasoning Framework
- Step-by-step reasoning process using REACT methodology
- Structured thought process with explicit reasoning, action, observation, and planning
- Dynamic adaptation to task complexity

### Tool Integration
- Seamless integration with external tools via JSON interface
- Built-in support for:
  - Calculator
  - Web Search
  - Weather API
  - Calendar Management
- Extensible architecture for custom tool addition

### Robust Error Handling
- Comprehensive error management system
- Automatic retry mechanisms
- Fallback strategies for tool failures
- Clear error documentation and recovery paths

## 🚀 Quick Start

```python
from swarms import Agent
from swarm_models import OpenAIChat

# Initialize the model
model = OpenAIChat(
    openai_api_key=your_api_key,
    model_name="gpt-4o-mini",
    temperature=0.1
)

# Create the agent
agent = Agent(
    agent_name="REACT-Agent",
    system_prompt=REACT_PROMPT,
    llm=model,
    max_loops="auto",
    output_type="string",
    streaming_on=True,
    interactive=True
)

# Run a query
response = agent.run("Your query here")
```

## 💡 Use Cases

### Financial Planning
```yaml
Example: "How can I establish a ROTH IRA to buy stocks and get a tax break?"

```

### Weather-Dependent Planning
```yaml
Example: "Should I plan a picnic for tomorrow?"
```

### Complex Calculations
```yaml
Example: "Calculate bulk order costs with tax"
```

### Schedule Management
```yaml
Example: "Find meeting times for team"
```

## 🛠 Technical Architecture

### YAML Configuration
- Agent capabilities and behavior defined in YAML
- Clear, maintainable configuration structure
- Easy modification of agent parameters

### JSON Tool Interface
```json
{
  "tool_call": {
    "name": "tool_name",
    "parameters": {
      "param1": "value1",
      "param2": "value2"
    }
  }
}
```

## 🔒 Best Practices

1. **Explicit Reasoning**
   - Clear thought process documentation
   - Structured decision-making
   - Traceable logic flow

2. **Tool Usage**
   - Precise parameter specification
   - Documented tool calls
   - Error handling for each interaction

3. **Process Management**
   - Clear phase separation
   - Detailed observation recording
   - Explicit next steps planning

## 📊 Performance Optimization

- Automatic loop management with `max_loops="auto"`
- Temperature control for consistent outputs
- Streaming support for real-time responses

## 🤝 Contributing

Contributions are welcome! Please read our contributing guidelines and submit pull requests to our repository.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

Built with [Swarms](https://github.com/kyegomez/swarms) framework
Powered by OpenAI's language models

