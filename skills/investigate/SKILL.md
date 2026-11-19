---
name: investigate
description: "Investigate one Afterchat support conversation with the code and the vault, then write the reply. Use when someone points at a specific customer chat or asks why something happened to a customer."
argument-hint: "<conversation id>"
---

Investigate Afterchat conversation $ARGUMENTS: get_conversation, search_vault for what we already say, then read the code (and our own data if you can reach it) to find the real answer. Write back what is specific to their account (add_note), a general vault entry if one was missing (propose_entry with code_refs), and a short bug brief in a note if you found a bug. Then write the reply for the customer (reply) with checked, what you looked at, and saved, what you wrote back, one short line each.
