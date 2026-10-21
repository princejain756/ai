---
'@ai-sdk/otel': patch
---

Name `invoke_agent` root spans after `gen_ai.agent.name` (the telemetry `functionId`) instead of the model id when a `functionId` is set, matching the OpenTelemetry GenAI semantic conventions. Spans without a `functionId` keep the model id.
