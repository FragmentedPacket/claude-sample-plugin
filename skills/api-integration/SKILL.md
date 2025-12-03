# API Integration Skill

This skill provides capabilities for integrating with external APIs in a secure and efficient manner.

## Description

The API Integration skill enables Claude to assist with designing, implementing, and troubleshooting API integrations. This includes REST APIs, GraphQL endpoints, and webhook configurations.

## Capabilities

- Design API request/response structures
- Implement authentication flows (OAuth, API keys, JWT)
- Handle error responses and retries
- Parse and transform API responses
- Generate API documentation
- Create API client implementations

## When to Use

This skill is automatically invoked when:
- Creating new API integrations
- Debugging API communication issues
- Designing API contracts
- Implementing webhook handlers
- Setting up API authentication

## Best Practices

1. **Security**: Always use environment variables for API keys and secrets
2. **Error Handling**: Implement proper error handling with meaningful messages
3. **Rate Limiting**: Respect API rate limits and implement backoff strategies
4. **Validation**: Validate request and response data
5. **Logging**: Log API calls for debugging (without sensitive data)

## Example Usage

When implementing an API integration:

```
Integrate with the GitHub API to fetch repository information
```

The skill will guide the implementation with:
- Appropriate authentication setup
- Request/response type definitions
- Error handling patterns
- Rate limiting considerations

## Resources

- REST API design guidelines
- OAuth 2.0 implementation patterns
- GraphQL query optimization
- Webhook security best practices
