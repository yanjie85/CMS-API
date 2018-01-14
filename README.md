# CMS-API
## Customer Management API for Fun

This a exercise that implement a RESTful API using RAML (http://raml.org) and MuleSoft (http://www.mulesoft.com) that contains a single resource, customer, and allows the following:
- List customers
- Create a new customer
- Update a customer
- Deletes a customer

The implementation make use of HTTP method determine which function to perform, the implementation as follow:

- Method  | Actions               | Url
- Get     | List customers        | http://localhost:8081/api/customers
- Post    | Create a new customer | http://localhost:8081/api/customers
- Put     | Update a customer     | http://localhost:8081/api/customers/{id}
- Delete  | Deletes a customer    | http://localhost:8081/api/customers/{id}
- Get     | List a customer       | http://localhost:8081/api/customers/{id}

### Database:
It uses ObjectStore to store customers information in the form of ObjectStore<ID : HashMap<Attribute:Value>>
