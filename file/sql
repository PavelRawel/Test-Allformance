SELECT *,

Case 
WHEN  last_click_source = '(direct) / (none)' and last_view_source  = 'no_source' then 'no source'
when last_click_source IN ('google / cpc', 'email / newsletter', 'awin / cpa', '(direct) / (none)') AND last_view_source IN  ('criteo / banner', 'google / cpm', 'no_source') then 'perf'
when last_click_source IN ('google / organic', '(direct) / (none)') AND last_view_source IN  ('youtube / video', 'no_source') then 'brand'
else 'mix'
 end as type
 from `test-380207.de2024.marketing`
