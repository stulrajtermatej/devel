# Developing and solving problems ...
## Eurostat Query builder
1. open database link: <a href="https://ec.europa.eu/eurostat/web/main/data/database">https://ec.europa.eu/eurostat/web/main/data/database</a>
2. open indictator from table: https://appsso.eurostat.ec.europa.eu/nui/show.do?dataset=prc_hicp_midx&lang=en
<br>2.1. Table ID is: prc_hicp_midx
3. open query builder: <a href="https://ec.europa.eu/eurostat/web/json-and-unicode-web-services/getting-started/query-builder">https://ec.europa.eu/eurostat/web/json-and-unicode-web-services/getting-started/query-builder</a>
4. insert table id click next
5. insert Geo selection=EA, unit=I15, coicop=CP00, click generate query filter
6. copy prc_hicp_midx?precision=1&geo=EA&unit=I15&coicop=CP00 and append into link like this http://ec.europa.eu/eurostat/wdds/rest/data/v2.1/json/en/prc_hicp_midx?precision=1&geo=EA&unit=I15&coicop=CP00
7. python use new link to download selected data and parse json output to pandas dataframe.
