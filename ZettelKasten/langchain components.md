202410031728
Status: #idea
Tags: [[agent]]

[Course](https://learn.deeplearning.ai/courses/langchain/lesson/3/memory)
# Models
- model contains prompt template, and can add parameters: reuse the prompt.
- has a pause (thought, action, thought, action) COT
- output parser: parse string/json to dict
# Memory
- control memory buffer: can set windows
- 
# Prompts

# Indexes

# Chains
Create a chain of actions
1. Simple Sequencial Chains: a flow with single input and single output.
2. SequentialChain: chain are connected by inputs, and outputs. The name of output and input must match. Both simple Sequencial chains and Sequential Chain have only one output. but Sequential Chain can have multiple input and Sequencial chains only have 1 input.
3. Router chain: 
	1. destination prompts: prompts and prompt info(name, description), + 1 default chain
	2. router: that used to select the destination prompt.

# Question and Answer over a Doc
1. Vector Store: vector store + loader. Just query. 
2. LLM: with the context put on the top of query.

# Agents
- Tools/Agents: Calculator, Wikipedia, Python Agent, 
- Action: one action need a tool name and action_input.
- 
# Evaluation
1. Looking by eyes
2. hard-code examples
3. LLM-generated examples
4. review by eyes
5. review by QAEvalChain
6. Turn on debug mode: to view what happen.