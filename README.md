# Grocery Brain

Grocery Brain is an ongoing agentic workflow project built in n8n to make grocery planning more structured and easier to manage.It started from a real problem I deal with myself: spending too much time trying to remember what is running low, what I already bought, and what needs to be restocked.

What began as a grocery planning project gradually became a way for me to explore how AI agents, workflow automation, routing logic, structured data, and human review can work together inside a business process.

## What It Does

Grocery Brain accepts a grocery-related request through chat, sends it to an AI agent, and then passes the output into workflow logic that helps determine the next step.

Instead of stopping at text generation, the workflow converts the result into structured fields that can be used for routing, ownership assignment, and review decisions.

## Current Features

* Chat-based intake in n8n
* AI-powered request analysis
* Conversational memory
* JavaScript code node for structured outputs
* Routing logic for workflow decisions
* Ownership assignment
* Human-review and escalation paths
* Workflow guardrails

## Workflow Overview

At a high level, the workflow:

1. Receives a grocery request
2. Passes the request to an AI agent
3. Converts the output into structured fields such as:

   * category
   * owner
   * nextAction
   * needsHumanReview
   * reason
4. Uses routing logic to determine the appropriate path
5. Sends the request through either a routine workflow path or a human-review path

## Example Routes

* Routine restock → Grocery Planner
* Budget-related request → Budget Reviewer
* Unclear or ambiguous request → Household Coordinator

## Why I Built It

I built Grocery Brain because I wanted to solve a problem I actually experience while also learning how agentic workflows work in a practical setting.

This project pushed me to think beyond "What answer should the AI give?" and focus more on:

* Classification
* Automation boundaries
* Review points
* Structured data
* Routing decisions

## What I Learned

The biggest lesson from this project is that the AI model is only one part of the solution.

The harder part is designing the process around the model through:

* Decision points
* Routing rules
* Guardrails
* Ownership
* Escalation paths
* Human oversight

That is what turns a response into a workflow.

## Current Status

This project is still in progress and continues to expand through ongoing development and testing.

One issue I am actively working through is the human-review branch, because some ambiguous requests routed through the routine path during testing when they should have been escalated.

## Planned Improvements

* Improve human-review routing logic
* Connect purchase history
* Add pantry or inventory context
* Incorporate budget information
* Support household preferences
* Explore grocery platform and store API integrations

## Tools Used

* n8n
* OpenAI Chat Model
* JavaScript
* Workflow Routing Logic
* Agentic AI Design
* Human-in-the-Loop Review Concepts

## Project Note

This repository represents an ongoing personal project built from my original idea and expanded through continuous iteration.

It also supported graduate coursework, but the concept, direction, and continued development are part of my broader personal portfolio in AI workflow design, automation, and business process thinking.
