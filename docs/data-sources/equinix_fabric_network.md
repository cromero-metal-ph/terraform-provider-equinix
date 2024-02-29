---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "equinix_fabric_network Data Source - terraform-provider-equinix"
subcategory: "Fabric"
description: |-
  Fabric V4 API compatible data resource that allow user to fetch Fabric Network for a given UUID
---

# equinix_fabric_network (Data Source)

Fabric V4 API compatible data resource that allow user to fetch Fabric Network for a given UUID

## Example Usage

```hcl
data "equinix_fabric_network" "network_data_name" {
  uuid = "<uuid_of_network>"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `uuid` (String) Equinix-assigned network identifier

### Read-Only

- `change` (Set of Object) Information on asset change operation (see [below for nested schema](#nestedatt--change))
- `change_log` (Set of Object) A permanent record of asset creation, modification, or deletion (see [below for nested schema](#nestedatt--change_log))
- `connections_count` (Number) Number of connections associated with this network
- `href` (String) Fabric Network URI information
- `id` (String) The ID of this resource.
- `location` (Set of Object) Fabric Network location (see [below for nested schema](#nestedatt--location))
- `name` (String) Fabric Network name. An alpha-numeric 24 characters string which can include only hyphens and underscores
- `notifications` (List of Object) Preferences for notifications on Fabric Network configuration or status changes (see [below for nested schema](#nestedatt--notifications))
- `operation` (Set of Object) Network operation information that is associated with this Fabric Network (see [below for nested schema](#nestedatt--operation))
- `project` (Set of Object) Fabric Network project (see [below for nested schema](#nestedatt--project))
- `scope` (String) Fabric Network scope
- `state` (String) Fabric Network overall state
- `type` (String) Supported Network types - EVPLAN, EPLAN, IPWAN

<a id="nestedatt--change"></a>
### Nested Schema for `change`

Read-Only:

- `href` (String)
- `type` (String)
- `uuid` (String)


<a id="nestedatt--change_log"></a>
### Nested Schema for `change_log`

Read-Only:

- `created_by` (String)
- `created_by_email` (String)
- `created_by_full_name` (String)
- `created_date_time` (String)
- `deleted_by` (String)
- `deleted_by_email` (String)
- `deleted_by_full_name` (String)
- `deleted_date_time` (String)
- `updated_by` (String)
- `updated_by_email` (String)
- `updated_by_full_name` (String)
- `updated_date_time` (String)


<a id="nestedatt--location"></a>
### Nested Schema for `location`

Read-Only:

- `ibx` (String)
- `metro_code` (String)
- `metro_name` (String)
- `region` (String)


<a id="nestedatt--notifications"></a>
### Nested Schema for `notifications`

Read-Only:

- `emails` (List of String)
- `send_interval` (String)
- `type` (String)


<a id="nestedatt--operation"></a>
### Nested Schema for `operation`

Read-Only:

- `equinix_status` (String)


<a id="nestedatt--project"></a>
### Nested Schema for `project`

Read-Only:

- `project_id` (String)
