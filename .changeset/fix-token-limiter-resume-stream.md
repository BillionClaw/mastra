---
'@mastra/core': patch
---n**Fixed**
- Fixed `TokenLimiterProcessor` incompatibility with `resumeStream`. The processor no longer throws an error when the message list is empty during resume operations. This allows `resumeStream` to work correctly when an InputProcessor is applied to an Agent, as messages are loaded from the snapshot during resume rather than being passed as new messages.
