<div align="center">

# **SmartOrders API**
## **Force-Creating an Order**
---
</div>

<br>

This command allows you to create an order through the API.

<br>

### **Parameters**

<div class="container">
  <ul class="responsive-table">
    <li class="table-header">
      <div class="col col-1">Name</div>w
      <div class="col col-2">Type</div>
      <div class="col col-3">Description</div>
    </li>
    <li class="table-row">
      <div class="col col-1" data-label="Name">Username</div>
      <div class="col col-2" data-label="Type">String</div>
      <div class="col col-3" data-label="Description">The name of the user. Can be gotten from Player.Name.</div>
    </li>
    <li class="table-row">
      <div class="col col-1" data-label="Name">Ordered Item's</div>
      <div class="col col-2" data-label="Type">String</div>
      <div class="col col-3" data-label="Description">The name of the user. Can be gotten from Player.Name.</div>
    </li>
    <li class="table-row">
      <div class="col col-1" data-label="Name">Cashier</div>
      <div class="col col-2" data-label="Type">String</div>
      <div class="col col-3" data-label="Description">The UserId of the player who will recieve the points. Can be gotten from Player.UserId</div>
    </li>
  </ul>
</div>

<br>

### **Response**

Coming Soon.

<br>

### **Example**

```lua
api.Orders:ForceCreate("sasial",{"MenuItem1","MenuItem2"},123)
```