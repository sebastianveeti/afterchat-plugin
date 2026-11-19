---
name: ship
description: "Tell everyone who asked for an Afterchat request that it shipped, and update the vault."
argument-hint: "[request number]"
disable-model-invocation: true
---

Request $ARGUMENTS is deployed; if no number was given, ask which one. Write a two-line note in plain words for the people who asked, then call ship. Use check_impact with the files the change touched and flag true, then update the affected entries with propose_entry, and any guide it names with propose_guide.
