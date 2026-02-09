# Glossary (Repo Excerpt)

For the full glossary, see: https://github.com/instance001/Whatisthisgithub/blob/main/GLOSSARY.md

This file contains only the glossary entries for this repository. Mapping tag legends and global notes live in the full glossary.

## Chattyv1.1
| Term | Alternate term(s) | Alt map | External map | Relation to existing terminology | What it is | What it is not | Source |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Chatty v1.1 | Chatty | ~ | ~ | Offline desktop assistant release | Ollama-driven local assistant using Mistral; boots with capsule prompt, stores conversation log in `memory.json`, uses `config.json` for model/capsule selection | Not cloud-based; not shipping model weights; not multi-user | Chattyv1.1/README.md; Chattyv1.1/Chattyv1.1.zip:Chattyv1.1/Chatty.py |
| Capsule (Chatty v1.1) | Symbound.txt | = | ~ | System prompt capsule | Text capsule loaded from `capsules/` to steer behavior | Not executable code; not enforced policy beyond prompt | Chattyv1.1/Chattyv1.1.zip:Chattyv1.1/Chatty.py |
| Memory log (Chatty v1.1) | memory.json | = | ~ | Session persistence | JSON list capturing conversation turns and boot log; trimmed to last ~2 exchanges when building prompt | Not vector/embedding memory; not encrypted | Chattyv1.1/Chattyv1.1.zip:Chattyv1.1/Chatty.py |
| Local generation endpoint | http://localhost:11434/api/generate | = | = | Ollama API | HTTP endpoint used for text generation with selected model | Not remote SaaS; requires local Ollama | Chattyv1.1/Chattyv1.1.zip:Chattyv1.1/Chatty.py |
| Config (Chatty v1.1) | config.json | = | ~ | Runtime config | Contains `model` and capsule path; auto-created if missing with defaults | Not a credentials store; no API keys required | Chattyv1.1/Chattyv1.1.zip:Chattyv1.1/Chatty.py |
