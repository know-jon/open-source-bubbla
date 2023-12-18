---
title: Welcome to Evidence
---

_Build polished data products with SQL and Markdown_

<BarChart
  data={currency_codes}
  x=currency_code
  y=value
  title = "Current max value during december"
/>

### Value in Text

The currency rate have been between **<Value data={swedish_currency} column=min_value/>** and **<Value data={swedish_currency} column=max_value/>** per EURO. 

### Big Value 
<BigValue data={swedish_currency} value=avg_value />

## Run SQL Queries

```sql currency_codes
SELECT
currency_code,
max(value) as value
FROM clouddb.main.obt_currency
where date > '2023-12-01' and sub_region = 'Northern Europe'
group by currency_code
LIMIT 20;
```

```sql swedish_currency
SELECT
max(value) as max_value,
avg(value) as avg_value,
min(value) as min_value
FROM clouddb.main.obt_currency
where date > '2023-12-01' and currency_code = 'SEK'
LIMIT 20;
```

<Alert status=info>  
To see the queries on a page, click the 3-dot menu at the top right of the page and Show Queries. You can see both the SQL and the query results by interacting with the query above.
</Alert>

> **More:** See [all components](https://docs.evidence.dev/components/all-components)