# EntityService Namespace

Gives you the ability to easily inject base orm services or binded virtual entity services for you:

| DSL | Description |
| :--- | :--- |
| entityService | Inject a BaseORMService object for usage as a generic service layer |
| entityService:{entity} | Inject a VirtualEntityService object for usage as a service layer based off the name of the entity passed in. |

```javascript
// Generic ORM service layer
property name="genericService" inject="entityService";
// Virtual service layer based on the User entity
property name="userService" inject="entityService:User";
```

