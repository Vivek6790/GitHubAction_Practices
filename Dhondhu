terraform {
  required_providers {
    azurerm = {
      source  = "hashicorp/azurerm"
      version = "4.80.0"
    }
  }
  backend "azurerm" {
    resource_group_name  = "revision_rg"
    storage_account_name = "revisionsa"
    container_name       = "revisioncontainer"
    key                  = "majnu.tfstate"
  }
}

provider "azurerm" {
  features {}
  subscription_id = "d45d303f-5dbd-4fbf-9adb-39c652a0547d"
}


resource "azurerm_resource_group" "rg" {
  name     = "sonam-rg"
  location = "east us"
}
