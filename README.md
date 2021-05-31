# re-execute-an-action-when-it-fails

Logic Apps allows to retry failed action executions with the retry policy described in the below link:
https://docs.microsoft.com/en-us/azure/logic-apps/logic-apps-exception-handling#retry-policies 
“A retry policy specifies whether and how the action or trigger retries a request when the original request times out or fails, which is any request that results in a 408, 429, or 5xx response”

However, there could be some scenarios where could be needed to retry the action execution for other error codes than the ones mentioned (408, 429, or 5xx). This document provides a work around for intermittent issues to allow to re-execute an action when the status code is not covered by the retry policy.
