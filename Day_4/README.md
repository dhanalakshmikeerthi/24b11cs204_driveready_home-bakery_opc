# Day 4 – Tools, Function Calling, Agents and Structured Data

## Overview

Today we learned how AI agents use tools and functions to perform real actions, how structured data can be validated, and how information can be stored in Google Sheets.

## What We Learned

| Idea | What We Learned |
|---|---|
| **Tools** | Tools are functions that allow an AI agent to get live information, perform actions, and complete exact tasks. |
| **Function Calling** | The AI model decides when a function is needed, the program executes it, and the result is returned to the model. |
| **Good Tools** | Tools should have clear `snake_case` names, type hints, and useful docstrings that explain when the tool should be used. |
| **create_agent** | `create_agent` combines the AI model, tools, and prompt to create an agent. The execution trace helps understand the steps taken by the agent. |
| **Rate Limits** | Rate limits control how frequently an API can be used. A `429` response means requests should be slowed down. Proper error handling and smaller tests can help. |
| **Pydantic** | Pydantic allows data fields, types, and validation rules to be defined. It helps reject invalid data before processing. |
| **Google Sheets** | Google Sheets can be used to store structured information. `append_row` adds a new row of data to the sheet. |
| **log_order** | An order logging function can validate the order, calculate the total, save the completed order, and then confirm it. |

## Function Calling Workflow

```text
User Request
     ↓
AI Agent
     ↓
Decides whether a Tool is Required
     ↓
Function Call
     ↓
Code Executes the Function
     ↓
Result Returned to Agent
     ↓
Agent Continues
     ↓
Final Response
```

## Tool Design

We learned that good tools should have:

- Clear and meaningful names
- `snake_case` naming
- Type hints
- Useful docstrings
- Clear instructions about when the tool should be used
- Proper input and output handling

## Structured Data with Pydantic

Pydantic helps define and validate structured data.

It allows us to specify:

- Fields
- Data types
- Validation rules

This helps prevent invalid data from being processed by the application.

## Google Sheets Integration

We learned how Google Sheets can be used as a simple storage system for agent-related data.

The `append_row` operation adds information as a new row, allowing records to be stored in an organized way.

## Order Logging

We learned that an order should be processed carefully before it is stored.

The general flow is:

```text
Check Order
    ↓
Calculate Total
    ↓
Validate Complete Data
    ↓
Save Order
    ↓
Confirm Order
```

The order should only be confirmed after the required information has been checked and successfully saved.

## Rate Limits

We learned that APIs may restrict the number or frequency of requests.

A **429 response** indicates that requests are being made too quickly or a rate limit has been reached.

To handle this properly:

- Slow down requests
- Use smaller tests
- Avoid unnecessary API calls
- Handle errors using `try/except`
- Use an appropriate API key

## Key Takeaways

- Tools allow AI agents to perform real actions.
- Function calling connects AI decisions with program functions.
- Well-designed tools need clear names, type hints, and documentation.
- `create_agent` combines models, tools, and prompts.
- Rate limits require controlled API usage and error handling.
- Pydantic helps validate structured data.
- Google Sheets can be used to store agent data.
- `append_row` can add new records to a sheet.
- Order logging should validate and complete the process before confirmation.

## Conclusion

Day 4 helped us understand how AI agents can move beyond generating text and perform practical tasks using tools and functions. We also learned about structured data validation, API rate limits, agent creation, and storing information in Google Sheets.
