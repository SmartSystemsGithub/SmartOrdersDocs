<div align="center">

# **SmartOrders API**
## **Force-Creating an Order**
---
</div>

<br>

This command allows you to create an order through the API.

<br>

### **Parameters**

| Name | Type | Description |
| ----------- | ----------- | ------- |
| Username | String | The name of the user. Can be gotten from `Player.Name`.
| Items Orders | array | The names of items that are being served. Please follow the code example.
| Cashier | Integer | The Cashier's UserId to give points to. Can be gotten from `Player.UserId`

<br>

### **Response**

Coming Soon.

<br>

### **Example**

```lua
api.Orders:ForceCreate("sasial",{"MenuItem1","MenuItem2"},123)
```