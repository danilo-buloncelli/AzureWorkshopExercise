# CmpAzureDemo
[![topmovers-dev](https://github.com/comparis/topmovers-azure/actions/workflows/develop_topmovers-dev.yml/badge.svg?branch=develop)](https://github.com/comparis/topmovers-azure/actions/workflows/develop_topmovers-dev.yml)
[![topmovers-ratings-dev](https://github.com/comparis/topmovers-azure/actions/workflows/develop_topmovers-ratings-dev.yml/badge.svg?branch=develop)](https://github.com/comparis/topmovers-azure/actions/workflows/develop_topmovers-ratings-dev.yml)

## Setup database

Two options: 
- Restore topmovers_local database on your local machine. You can find a copy of it here: S:\ivan.radovic\sqlbackup and use `topmovers_local.bak`
- Change connection string in Web.config to point to Azure dev database. You can find dev connection string in the Web.Dev.config file or you can go to Azure portal and get connection string from `comparis-mkp-dev001` database.

### Azure App url
- Topmovers dev: https://topmovers-dev.azurewebsites.net/
- Topmovers dev test (temp): https://topmovers-dev-test.azurewebsites.net/
- Topmovers ratings dev: https://topmovers-ratings-dev.azurewebsites.net/

## Requirements
- .NET Framework 4.8
- Entity Framework 6.4.4
