# Decision Drift Auditor

An AI agent that detects when organizational decisions change, conflict, or become inconsistent across meetings, documents, messages, and other sources.

## Problem

Teams make decisions across meetings, documents, messages, and code changes. Later statements can silently contradict earlier decisions, creating confusion and inconsistent execution.

## Solution

Decision Drift Auditor extracts decisions, builds a timeline of changes, detects contradictions, and highlights decisions that require human confirmation.

## Example

Original decision:
"We will use PostgreSQL as the source of truth for customer data."

Later statement:
"The customer service application now uses MongoDB as its source of truth."

The agent flags this as potential decision drift and provides the evidence supporting the conflict.

## Status

Work in progress.
