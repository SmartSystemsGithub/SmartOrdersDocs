<div align="center">

# **SmartOrders API**
## **Force-Creating an Order**
---
</div>

<style>
body {
  font-family: 'lato', sans-serif;
}
.container {
  max-width: 1000px;
  margin-left: auto;
  margin-right: auto;
  padding-left: 10px;
  padding-right: 10px;
}

.responsive-table {
  li {
    border-radius: 3px;
    padding: 25px 30px;
    display: flex;
    justify-content: space-between;
    margin-bottom: 25px;
  }
  .table-header {
    background-color: #95A5A6;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 0.03em;
  }
  .table-row {
    background-color: #ffffff;
    box-shadow: 0px 0px 9px 0px rgba(0,0,0,0.1);
  }
  .col-1 {
    flex-basis: 25%;
  }
  .col-2 {
    flex-basis: 25%;
  }
  .col-3 {
    flex-basis: 50%;
  }
  
  @media all and (max-width: 767px) {
    .table-header {
      display: none;
    }
    .table-row{
      
    }
    li {
      display: block;
    }
    .col {
      
      flex-basis: 100%;
      
    }
    .col {
      display: flex;
      padding: 10px 0;
      &:before {
        color: #6C7A89;
        padding-right: 10px;
        content: attr(data-label);
        flex-basis: 50%;
        text-align: right;
      }
    }
  }
}
</style>

<br>

This command allows you to create an order through the API.

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