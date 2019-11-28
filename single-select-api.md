# Single select API

To enable the the API, add a custom field of value type Single select (API). 
This will create an API endpoint to insert values for that custom field. 

###API call

The API accepts only `POST` requests. You should send `list_values` along
with the `authenticator` which is an authentication token generated and displayed to you
when custom field is created. 

An example API call using CURL: 

```
curl -X POST https://stagingapi.risqover.com/webhook/customfields/api-values -H 'Content-Type: application/json' -d '{"authenticator": "1_r3222iy", "list_values": ["alpha", "beta"]}'
```

