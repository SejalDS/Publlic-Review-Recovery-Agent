
# Public Review Recovery Agent
An idea for an AI agent that watches public review sites for SharkNinja complaints, finds the customer, and hands the CX team a one-click recovery action — fast enough that customers often update their review.

Live prototype → https://sejalds.github.io/Publlic-Review-Recovery-Agent/

## The idea
SharkNinja's Good Call program does great work for customers who reach out. But many customers skip the call and post on Trustpilot, BBB, or Amazon instead. Those reviews shape the public score and reach future buyers — and Agentforce, by design, doesn't see them.
This agent extends Agentforce into that gap.

## How it works

![Image](https://github.com/SejalDS/Publlic-Review-Recovery-Agent/blob/main/Public%20Review%20Agent.png)

### Sources — watches Trustpilot, BBB, Amazon, Reddit for new complaints.

### Agent — classifies urgency, then uses the Salesforce Agentforce API to match the reviewer to a customer record and pull their order history. Drafts a recovery action on top of that data.

### Routing — pushes the case back into the existing Agentforce dashboard for one-click human approval, and sends pattern signals to product safety, ops, or legal.

## Why it builds on what's already there

Rather than replacing anything, the agent uses Agentforce as the system of record. Customer matching, ticket creation, and action execution all happen through Agentforce APIs — the CX team works in the same dashboard they already use. The agent just feeds it customers it couldn't see before.

## Prototype
The demo runs the workflow on 12 real, public reviews from 2023–2026. Customer match data is illustrative.

## About
Built independently as a study, inspired by the Jailbreak SharkNinja AI challenge.
