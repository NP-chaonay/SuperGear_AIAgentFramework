# SuperGear_AIAgentFramework
AI Agent Framework that opens your eyes by our interesting features; written in Python, intended to support various model backend.

## Drafting Specification
### Setup
1) User put Python Code that connect Model Backend into our system
2) Open our frontend
3) Add/Select Workspace (separating configuration/chat/data)
4) Add/Select Model Backend to use (can be local/cloud... can be multiple)
5) Let user to enabling/and setup Entity Orchestrator (useful for limited resource local model or limited cost of cloud model)
-) Our system: loaded model can be shared by Entity/EO/workspace but in FIFO policy... in case you want to enforce different switching policy... enabling Entiity Orchestrator and let the EO (decision tree fixed rule + LLM editing rule + LLM manage directly) manage
6) Add Agent and choose what Entity/EO (you may want to use EO instead I suggest lmao) to tie
7) <TBA>

- if user want to let AI entiities use same session of loaded model... user must implment Entities Orchestrator (The leader of all entities) that control who (ai entities) will got moment to use that model ... in case your computer does not have much resource for simultaneously running model for each entities and not want to pay for cloud AI

- autonomous operation where many AI entity talk on their own and do their work... without asking user unless Entity think it should or it met condition that user have told  

- while agent chat on its own... agent can receive message/instruction from user too (and user can set a flag that make agent pause the chat and focus to user request first)

- while tool executing ... agent can chat without wait... agent can monitor the tool progress/output when agent want ... (if agent want to do perodic monitoring... agent can use "timer" tool)... tool can trigger agent to wakeup too (such as file/internet/command operation finished/failed) 
```
and now you know why I plan to make the new framework... Gemini Flash HighThink told me that I should make it
