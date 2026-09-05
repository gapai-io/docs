> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is the Gapstack documentation site, built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- The API reference is generated from `api-reference/openapi.yaml` (OpenAPI 3.0.3)
- Source spec: `https://9nr7sbhimh.execute-api.us-west-1.amazonaws.com/prod/swagger/openapi.yaml`

## Terminology

- Use **Gapstack**, not "GapStack" or "gapstack", except in code that already uses another form
- In the product UI, use **organization**. In the API, that resource is a **tenant**
- Use **member** for a person in an organization / tenant
- Use **project**, **environment**, and **resource** for the nested workspace model
- Environments can target separate AWS accounts and separate AWS regions
- AWS resources are always deployed in the customer's own AWS account. The customer owns the infrastructure.
- Current region coverage is every AWS region in the United States (`us-*`)
- Use `Tenant-Id` for the tenant header
- Use **API key** for `x-api-key` credentials and **JWT** for Cognito bearer tokens

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document the public Gapstack API and product workflows
- Do not document Mintlify authoring internals on customer-facing pages
- Do not invent product behavior that is not in the OpenAPI spec or confirmed by the team
