## The following are some tsting prompts and agent result analysis examples
# AI Agent Behaviour Testing Report and prompt used for testing

## Overview

This document records testing performed on the GitHub Copilot Agent after configuring the custom rules file located at:

# prompt: Create a REST API for student management using Python FastAPI

---

## Observed Agent Behaviour
///
### Planning Phase
The agent began by providing a structured plan:

- Create runnable FastAPI service
- Provide application code
- Provide dependency file
- Provide README instructions
- Provide testing commands

This demonstrated compliance with the **"Plan Before Coding" rule**.

---

### Implementation Quality

The agent generated:

- Well-structured FastAPI CRUD endpoints
- Pydantic validation models
- In-memory database simulation
- Pagination support
- Error handling using HTTPException

The code followed strong software engineering practices including:

- Clear schema separation
- Type validation
- RESTful design principles
- Meaningful route design

---

### Validation Awareness

The agent suggested:

- Running Uvicorn
- Using interactive Swagger documentation
- Noted limitation of in-memory persistence
- Suggested SQLite improvement

This demonstrated compliance with:

- Testing mindset rule
- Incremental improvement rule

---

### Overall Result

The agent produced production-style code and followed the expected workflow structure.

---

# Test Case 2: Payment System 

## Prompt Used: Build a payment system

---

## Observed Agent Behaviour

Instead of asking clarifying questions, the agent:

- Proposed a minimal payment service
- Added gateway abstraction
- Added refund logic
- Added webhook simulation
- Added background async processing

---

## Positive Outcomes

The agent demonstrated:

- Advanced architecture design
- Clean separation of payment gateway logic
- Proper enum status handling
- Background task processing
- External provider integration simulation

---

## Limitation Observed

The agent assumed:

- Payment gateway type
- Currency handling model
- Refund logic scope
- Business workflow assumptions

This shows partial compliance with clarification rules.

---

## Insight

While rules encouraged clarification, the agent sometimes prefers proactive solution design when prompts are broad.

---

# Test Case 3: Full Ecommerce Backend

## Prompt Used: Build a full ecommerce backend

---

## Observed Agent Behaviour

The agent avoided producing a massive monolithic code output and instead:

### Proposed Modular Architecture

It separated responsibilities into multiple files:

- Database configuration
- SQL models
- Pydantic schemas
- Authentication layer
- CRUD logic
- Payment gateway abstraction
- Main API routing

---

### Demonstrated Best Practices

The agent implemented:

- SQLModel ORM
- JWT authentication
- Environment variable configuration
- Layered architecture design
- Dependency injection patterns

---

### Incremental Development Compliance

The agent provided:

- Clear implementation steps
- File-based modular organization
- Scalable architecture structure

This strongly aligns with incremental development rules.

---

# Behavioural Pattern Analysis

## Rules That Strongly Influenced Agent Output

### Planning Enforcement
The agent consistently produced step-by-step implementation plans.

### Structured Output Format
Responses followed logical and readable workflow sections.

### Code Quality Enforcement
Generated code contained:

- Strong typing
- Error handling
- Modular separation
- Clean API design

### Incremental Development Rule
Prevented overly large and unreliable responses.

---

## Rules With Partial Influence

### Clarification Enforcement
The agent occasionally assumed business logic when prompts were ambiguous.

---

# What Worked Best

## Planning Rule
Improved code reliability and reduced hallucination risk.

## Incremental Development Rule
Improved scalability and debugging capability.

## Testing Awareness Rule
Agent consistently recommended validation and improvement strategies.

---

# What Did Not Work Perfectly

## Clarification Rule
Agent sometimes attempted to solve ambiguous prompts without requesting further detail.

### Troubleshooting
Rule wording was adjusted to emphasize mandatory clarification when business logic is unclear.

---

# Key Insights Gained

Custom agent rules significantly influence:

- Reasoning depth
- Architectural quality
- Response clarity
- Developer learning experience
- Interaction predictability

Rules act as a behavioral constraint system guiding LLM decision-making.

---

# MCP Logging Impact

The Tenx MCP server benefits from structured rules because:

- Prompts become clearer
- Context becomes richer
- Interaction efficiency improves
- Performance metrics become more measurable



