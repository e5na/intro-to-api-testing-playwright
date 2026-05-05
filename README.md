# Checklist for GET /test-orders/auth

| Scenario name                                                    | Test data                       |
|------------------------------------------------------------------|---------------------------------|
| GET auth returns API key and login message with<br/> RC=200      | username=test<br/>password=test |
| GET auth returns RC=500 and message username or password missing | username=''<br/>password=''     |

# Checklist for PUT /test-orders/{id}

| Scenario name                                | Test data         |
|----------------------------------------------|-------------------|
| PUT request returns RC=200 and updated order | orderId = 7       |
| PUT request returns RC=401                   | incorrect api key |

# Checklist for DELETE /test-orders/{id}

| Scenario name                 | Test data    |
|-------------------------------|--------------|
| DELETE request returns RC=204 | orderId = 8  |
| DELETE request returns RC=401 | api_key = '' |