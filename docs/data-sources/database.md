---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "astra_database Data Source - terraform-provider-astra"
subcategory: ""
description: |-
  astra_database provides a datasource for Astra an Astra database. This can be used to select an existing database within your Astra Organization.
---

# astra_database (Data Source)

`astra_database` provides a datasource for Astra an Astra database. This can be used to select an existing database within your Astra Organization.

## Example Usage

```terraform
data "astra_database" "db" {
  database_id = "8d356587-73b3-430a-9c0e-d780332e2afb"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **database_id** (String) Astra Database ID (system generated)

### Optional

- **id** (String) The ID of this resource.

### Read-Only

- **additional_keyspaces** (List of String) Additional keyspaces
- **cloud_provider** (String) Cloud provider (AWS, GCP, AZURE)
- **cqlsh_url** (String) URL for cqlsh web
- **data_endpoint_url** (String) REST API URL
- **grafana_url** (String) URL for the grafana dashboard for this database
- **graphql_url** (String) Graphql URL
- **keyspace** (String) Initial keyspace
- **name** (String) Database name (user provided)
- **node_count** (Number) Node count (not relevant for serverless databases)
- **organization_id** (String) Ordg id (system generated)
- **owner_id** (String) Owner id (system generated)
- **regions** (List of String) Cloud provider region. Get list of supported regions from regions data-source
- **replication_factor** (Number) Replication Factor (not relevant for serverless databases)
- **status** (String) Database status
- **total_storage** (Number) Storage Capacity (not relevant for serverelss databases)


