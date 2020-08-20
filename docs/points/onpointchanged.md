<div align="center">

# **SmartOrders API**
## **On Point Changed**
---
</div>
 
<br>

This command detects when a player's point's has changed through the API.

<br>

### **Parameters**

| Name | Type | Description |
| ----------- | ----------- | ------- |
| Callback Function | Function | The function that will be ran when the point has changed.

<br>

### **Response**

| Name | Type | Description |
| ----------- | ----------- | ------- |
| isManual | Boolean | If this is false, it means that the point was updated by SmartOrders.
| pointAmount | Integer | The amount of points the user has.
| player | PlayerObject | The player that has had the points updated.

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