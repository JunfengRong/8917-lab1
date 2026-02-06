1. install requirements
```
pip install -r requirements.txt
```

2. configure variables in local.settings.json
- DATABASE_CONNECTION_STRING: connection string to your Cosmos DB
- COSMOS_DATABASE: name of your Cosmos DB database
- COSMOS_CONTAINER: name of your Cosmos DB container

example local.settings.json
```json
{
  "IsEncrypted": false,
  "Values": {
    "FUNCTIONS_WORKER_RUNTIME": "python",
    "AzureWebJobsStorage": "UseDevelopmentStorage=true",
    "DATABASE_CONNECTION_STRING": "",
    "COSMOS_DATABASE": "",
    "COSMOS_CONTAINER": ""
  }
}
```

1. run locally
```
func start
```

