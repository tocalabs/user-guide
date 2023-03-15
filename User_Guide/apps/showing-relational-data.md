
# Showing Relational Data

Showing Relational Data is critical once you're using TablesV3 and have created Related Data in your datastore.

Dynamic Data Provider is the answer!

_For this guide, I assume there's already and app, and you're on a Dynamic Page with a datastore and with relational data setup. See [Dynamic-pages](./User_Guide/dynamic-pages) for help getting to this point._

1. Select `Dynamic data wrapper` from the Components panel and drag into your page

2. Select `Data Source` - this should be the related item, not the item which is already linked in the Dynamic Page config.

3. Enter the Column/Property in the related Data Source (from step 2) - this is the field in the related table which is the Foreign Key to our Dynamic Page Datasource

4. Select Data ID - which is the other end of Foreign Key link, from the Context tab in the Datachip selector (or any other property you have)

