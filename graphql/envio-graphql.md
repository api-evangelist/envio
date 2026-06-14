# Envio GraphQL API

The Envio HyperIndex GraphQL API exposes indexed smart contract events and blockchain state from any EVM-compatible chain. Each HyperIndex deployment auto-generates a GraphQL API based on the user-defined `schema.graphql` entities, backed by a Hasura engine. The API supports queries, subscriptions (via WebSockets), filtering, sorting, and pagination over indexed on-chain data. Built-in system types provide indexing progress and metadata alongside user-defined entity types.

**Endpoint:** `https://indexer.hyperindex.xyz/{deployment-id}/graphql`

Local development endpoint: `http://localhost:8080/v1/graphql`

WebSocket endpoint: `wss://indexer.hyperindex.xyz/{deployment-id}/graphql` (swap `https://` to `wss://`)

**Authentication:** Bearer token via the `ENVIO_API_TOKEN` environment variable, required for HyperSync services. Envio Cloud-deployed indexers include access without a custom token.

**Documentation:** https://docs.envio.dev/docs/HyperIndex/overview

**References:**
- Documentation: https://docs.envio.dev/docs/HyperIndex/overview
- GettingStarted: https://docs.envio.dev/docs/HyperIndex/schema.md
- Schema: https://docs.envio.dev/docs/HyperIndex/schema.md
- Authentication: https://docs.envio.dev/docs/HyperSync/api-tokens
- MetadataQuery: https://docs.envio.dev/docs/HyperIndex/metadata-query.md
- QueryConversion: https://docs.envio.dev/docs/HyperIndex/query-conversion.md
- WebSockets: https://docs.envio.dev/docs/HyperIndex/websockets.md
- HasuraConsole: https://docs.envio.dev/docs/HyperIndex/navigating-hasura.md
