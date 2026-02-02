---
name: remembering-conversations
description: >
  Search past Claude Code conversations for context, decisions, and solutions.
  Triggers: "last time", "before", "we discussed", "dernière conversation",
  "la dernière fois", "on avait fait", "tu te souviens", "do you remember",
  "what did we work on", "qu'est-ce qu'on a fait", "notre dernière session",
  "previous session", "we talked about", "rappelle-toi", "remember when",
  "past work", "travail précédent", "session précédente", "notre dernier travail",
  "what was our last task", "quelle était notre dernière tâche".
  Also use after exploring code when stuck or making architectural decisions.
argument-hint: [search query or topic]
context: fork
agent: episodic-memory:search-conversations
allowed-tools: Bash
---

# Search Request

Search episodic memory for: $ARGUMENTS

Focus on:
- Decisions made and their rationale
- Solutions that worked (or didn't)
- Patterns, gotchas, and lessons learned
- Relevant code approaches

Return a synthesis (200-1000 words) with source references.
