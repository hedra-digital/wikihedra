# For Odoo admin users

## Queries

```sql
/*Queries I used, (will add some more in the future while working for edlab
stock)*/
UPDATE stock_move AS sm**
SET state = 'cancel'
FROM stock_picking AS sp
WHERE sp.id = sm.picking_id and sp.state = 'cancel' and sm.state != 'cancel'
and sm.company_id=24;

/* Canceled transfers whose the stock moves are not canceled*/
Select sm.id, sm.state, sp.id, sp.name, sp.state
From stock_move as sm 
JOIN stock_picking as sp ON sp.id=sm.picking_id
WHERE sp.state = 'cancel' and sm.state != 'cancel';
IGNORE this message

/* Canceled stock moves whose the product moves are not canceled*/
select sm.id, sml.id, sml.state
from stock_move_line as sml
join stock_move as sm
on sm.id=sml.move_id
where sm.state='cancel' and sm.company_id=24 and sml.state != 'cancel';
```

