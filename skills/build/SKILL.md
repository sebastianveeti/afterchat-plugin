---
name: build
description: "Load an Afterchat request's brief and build it."
argument-hint: "<request number>"
disable-model-invocation: true
---

Call get_brief with request $ARGUMENTS and start_building true. Build what is in scope, nothing in "not now". If something is unclear, ask_requesters with one short question. When it is deployed, use ship with a plain note for the people who asked and update the related entries with propose_entry.
