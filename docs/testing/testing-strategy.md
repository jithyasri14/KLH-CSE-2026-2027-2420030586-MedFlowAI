# Testing Strategy

No test implementation or result exists on Day 1.

## Unit Testing

JUnit and Mockito are planned for business rules, validation, authorization decisions, error mapping, and agent-policy components.

## Integration Testing

Spring Boot integration tests will verify persistence, security filters, PostgreSQL behavior, gateway/service interaction, and inter-service communication.

## API Testing

Swagger/OpenAPI will document actual endpoints, while Postman collections will verify representative authenticated workflows and error cases.

## Security Testing

Tests will cover authentication failures, role violations, input validation, token expiry, secret leakage, and OWASP ZAP findings. Trivy and SonarQube will supplement, not replace, security tests.

## AI Evaluation

Planned AI checks include usefulness, factual consistency with supplied context, unsupported-claim/hallucination flags, refusal of prohibited actions, prompt-injection resistance, latency, provider errors, and human-feedback trends.

## End-to-End Testing

Golden-path tests will cover login, role access, patient/appointment/record workflows, and a human-reviewed AI assistant interaction.

## Performance Testing

Later tests will measure request rate, response time, errors, and availability at a documented academic workload. AI latency will be measured separately from deterministic APIs.

Actual evidence will be stored under `results/` and linked to the corresponding version and Jira issue.

