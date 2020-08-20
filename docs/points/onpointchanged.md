<div align="center">

# **SmartOrders API**
## **On Point Changed**
---
</div>
 
<br>

This command detects when a player's point's has changed through the API.

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
      <div class="col col-1" data-label="Name">Callback Function</div>
      <div class="col col-2" data-label="Type">Function</div>
      <div class="col col-3" data-label="Description">The function that will be ran when the point has changed.</div>
    </li>
  </ul>
</div>


<br>

### **Response**

<div class="container">
  <ul class="responsive-table">
    <li class="table-header">
      <div class="col col-1">Name</div>
      <div class="col col-2">Type</div>
      <div class="col col-3">Description</div>
    </li>
    <li class="table-row">
      <div class="col col-1" data-label="Name">isManual</div>
      <div class="col col-2" data-label="Type">Boolean</div>
      <div class="col col-3" data-label="Description">If this is false, it means that the point was updated by SmartOrders.</div>
    </li>
    <li class="table-row">
      <div class="col col-1" data-label="Name">pointAmount</div>
      <div class="col col-2" data-label="Type">Integer</div>
      <div class="col col-3" data-label="Description">The amount of points the user has.</div>
    </li>
    <li class="table-row">
      <div class="col col-1" data-label="Name">player</div>
      <div class="col col-2" data-label="Type">PlayerObject</div>
      <div class="col col-3" data-label="Description">The player that has had the points updated.</div>
    </li>
  </ul>
</div>


<br>

### **Examples**

<br>

## Point Bonus
```lua
-- This example is so that if they get 1 point from SO, it'll give another.
api.Points.OnPointChanged:Connect(function(isManual,pointAmount,player)
 if isManual == true then 
    -- This is where if the points was updated by a in-game script, not SmartOrders, it'll return true.
    return 
 end
 print("Point added by SO.")
 api.Points:Add(player.UserId,1) 
end)
```
<br>

## Checking Points
```lua
api.Points.OnPointChanged:Connect(function(isManual,pointamount,player)
 if pointamount % 150 then
  -- Promo time! As the point amount is divisble by 150.
  end
end)
```