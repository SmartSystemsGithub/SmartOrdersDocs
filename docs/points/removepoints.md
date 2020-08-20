<div align="center">

# **SmartOrders API**
## **Removing Points**
---
</div>

<br>

This command allows you to remove points through the API.

<br>

### **Parameters**

<div class="container">
  <ul class="responsive-table">
    <li class="table-header">
      <div class="col col-1">Name</div>
      <div class="col col-2">Type</div>
      <div class="col col-3">Description</div>
    </li>
    <li class="table-row">
      <div class="col col-1" data-label="Name">UserId</div>
      <div class="col col-2" data-label="Type">Integer</div>
      <div class="col col-3" data-label="Description">The ID of the user. Can be gotten from `Player.UserId`.</div>
    </li>
    <li class="table-row">
      <div class="col col-1" data-label="Name">Points</div>
      <div class="col col-2" data-label="Type">Integer</div>
      <div class="col col-3" data-label="Description">The amount of points to remove from the user.</div>
    </li>
  </ul>
</div>

<br>

### **Response**

Coming Soon.

<br>

### **Example**

```lua
api.Points:Remove(123,1)
```