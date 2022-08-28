SELECT NAME
ROUND(1.0 * count{distinct order.id}/
    count( distinct order.delivered_to), 2)
    as reorder_rate
    FROM ORDER_itens
    join ORDER ON
    order.id = order_items.order_id
    GROUP BY 1
    GROUP BY 2 DESC

select mods.tags.value, Count(*) AS num
from nodesTags
JOIN(select distinct (id))
FROM nodesTags
WHERE VALUE = 'Bank')
on nodesTags.id=i.ID
WHERE nodestags.KEY= "name"
GROUP BY nodestags.VALUE
order BY num DESC
limit 5;
