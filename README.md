# Nishanth Module Introduction.

This document will help you to understand the functionality of the Nishanth Static Website module.

Here are some code sample on how to use this module.

```hcl
module "nishanth_static_website" {
    source = "./modules/azure-static-website" # Mandatory, and Folder Name with Path

    resource_group_name = "myrg1"
    location = "eastus"

    storage_account_name = "stweb93430"

    storage_account_tier = "Standard"

    storage_account_replication_type = "LRS"

    storage_account_kind = "StorageV2"

    static_website_index_document = "index.html"

    static_website_error_404_document = "error.html"

}
```