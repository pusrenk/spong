# spong
Sistem PengelOlaan uaNG



current structure use combination of Domain-Driven Design (DDD) and Clean Architecture
reason : to make it scaleable along with the ability seperate each business logic

```bash
📦 spong
├─ src
│  └─ transaction
│     ├─ handlers
│     │  ├─ http
│     │  │  └─ transaction.rs // this one is for request controller with restful http
│     │  └─ rpc
│     │     └─ transaction.rs // this one is for request controller with rpc
│     ├─ services
│     │  └─ transaction.rs // this one we can call usecase/domain layer
│     ├─ storage/repository
│     │  └─ transaction.rs // this one we can call data layer
│     ├─ entity
│     │  └─ transaction.rs // this one is for entity of the domain
│     └─ models
│        ├─ request.rs // this one is for request payload
│        └─ response.rs // this one is for response payload
└─ pkg
   ├─ database
   │  └─ database.rs // db config
   └─ utils
      └─ logger.rs // log function to be used at at fn
      └─ constant.rs // all possible global var that not dynamically change can be store here to make it cleaner
```