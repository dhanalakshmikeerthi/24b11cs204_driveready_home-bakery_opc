# Day 3 – AI Agents, Tools, Memory and Agent Loop

## Overview

Today we learned the basic components of an AI Agent and how an agent works step by step to complete a task.

## What We Learned

### 1. Components of an AI Agent

An AI agent is built using four important parts:

- **Brain** – The LLM that understands the task and decides what to do.
- **Instructions** – The system prompt that guides the agent's behavior.
- **Tools** – Functions that the agent is allowed to call to perform actions.
- **Memory** – Information from previous interactions that helps the agent remember relevant details.

These four parts work together to make an AI agent useful and capable of performing tasks.

### 2. Brain – LLM

The **LLM (Large Language Model)** acts as the brain of the agent.

It understands the user's request, processes the available information, and decides the next step required to complete the task.

### 3. Instructions – System Prompt

The **system prompt** provides instructions to the agent.

It controls how the agent should behave, what it should do, and how it should respond.

Clear instructions help the agent follow the required behavior instead of making random decisions.

### 4. Tools

Tools are **functions that an agent is allowed to call** to perform specific actions.

Tools allow an agent to do more than simply generate text.

The agent can decide when a tool is required and use its result to continue working toward the goal.

### 5. Memory

Memory allows an agent to retain relevant information from previous interactions.

It helps the agent maintain context instead of forgetting information from earlier parts of a conversation.

Without memory, an agent may lose important information from previous interactions.

---

# Agent Loop

## Think → Act → Observe → Repeat

We learned that an AI agent generally works through a continuous loop.

### 1. Think

The agent determines what needs to be done next based on the user's goal and the available information.

### 2. Act

The agent decides to perform an action, such as calling an available tool.

### 3. Observe

The tool performs the requested action and returns a result.

The agent receives this result and uses it to decide what to do next.

### 4. Repeat

The agent continues the **Think → Act → Observe** cycle until the required goal is completed.

### 5. Final Answer

When the agent has enough information to complete the task, it stops the loop and provides the final response.

---

## ReAct Pattern

This agent workflow is commonly associated with the **ReAct (Reason + Act)** pattern.

The basic flow is:

```text
User Goal
    ↓
Think
    ↓
Act
    ↓
Tool
    ↓
Observe Result
    ↓
Think Again
    ↓
Act Again
    ↓
Final Answer
```

The loop continues until the agent reaches the required result or the execution is stopped after too many rounds.

---

## Key Takeaways

- An AI agent combines a **brain, instructions, tools, and memory**.
- The LLM acts as the brain of the agent.
- System prompts provide instructions and control the agent's behavior.
- Tools allow the agent to perform actions.
- Memory helps the agent retain relevant information.
- An agent works through a **Think → Act → Observe → Repeat** loop.
- The ReAct pattern combines reasoning and actions.
- The agent can use tool results to decide its next step.
- The loop ends when the agent reaches the required goal and produces a final answer.

## Conclusion

Today we understood the basic structure and working process of AI agents. We learned how the LLM, system instructions, tools, and memory work together. We also learned how an agent can repeatedly think, perform actions, observe results, and continue until the required task is completed.
