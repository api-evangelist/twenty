# Twenty CRM GraphQL API

Twenty exposes two GraphQL endpoints for every workspace: the Core API at `/graphql` and the Metadata API at `/metadata`. The Core API is schema-per-tenant — the types and fields available at query time reflect the standard objects (Company, Person, Opportunity, Note, Task, WorkspaceMember, Workflow, Attachment, and more) plus any custom objects the workspace has defined. All schema extensions made through the Metadata API are immediately reflected in the Core API surface, making the GraphQL schema fully dynamic. Each object type generates a standard suite of query fields (findOne, findMany, findDuplicates, groupBy) and mutation fields (createOne, createMany, updateOne, updateMany, deleteOne, deleteMany, restoreOne, restoreMany, destroyOne, destroyMany, mergeMany).

Authentication against both endpoints uses a Bearer token scoped to a workspace. Tokens are generated from the workspace's Security settings page (Settings → Security → API Keys) or via the Authentication API. For cloud users the endpoints are hosted at `https://api.twenty.com`; self-hosted deployments expose the same paths on their own domain. Both endpoints accept `Authorization: Bearer <token>` in the request header. The Metadata API additionally requires the same token but operates on schema objects (object metadata, field metadata, relation metadata) rather than CRM records.

The GraphQL schema is generated dynamically at runtime by the workspace-schema-builder, which converts each workspace entity definition — including composite field types such as FullName, Emails, Phones, Links, Currency, Address, and RichText — into corresponding GraphQL object types, filter input types, order-by input types, and connection types following the Relay cursor-connection specification. Batch operations accept up to 60 records per request. Filtering supports equality, string matching, date ranges, and nested relation filters. The Metadata API exposes its own GraphQL surface for programmatic CRUD on ObjectMetadata, FieldMetadata, RelationMetadata, and IndexMetadata entities.

**Endpoint:** https://api.twenty.com/graphql

**Metadata Endpoint:** https://api.twenty.com/metadata

**Documentation:** https://docs.twenty.com/developers/extend/api

**References:**

- Documentation: https://docs.twenty.com/developers/extend/api
- GettingStarted: https://docs.twenty.com/developers/introduction
