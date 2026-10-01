# MarketsEasy for Claude

MarketsEasy runs marketplace operations for suppliers that sell on European marketplaces such as bol, Kaufland and Allegro. This plugin connects Claude to your MarketsEasy account, so you can ask about orders, products and marketplace status in plain language, and let Claude prepare changes that you approve in MarketsEasy.

## What you can do

- Find orders across the suppliers you can access, filter them by order date, and open one order's status, tracking and carrier.
- Look up products, prices and stock, and check listing health and product discovery results.
- Propose changes, such as creating or updating an order or a product, adding tracking, or editing a warehouse. Every change waits for a person to approve it in MarketsEasy under **Agents & access**, and runs only after that approval.

Claude can only see and propose what your own MarketsEasy account is allowed to do. You need a MarketsEasy account to use this plugin.

## Connect

1. Add the plugin in Claude, then connect **MarketsEasy** on the plugin's **Connectors** tab. In Claude Code the connection starts when you first use a MarketsEasy tool.
2. Sign in with your MarketsEasy account at `auth.marketseasy.com` and allow the connection.
3. Ask, for example: "Show my MarketsEasy orders from the last 7 days" or "Which products are low on stock?"

You can see and disconnect your connections in MarketsEasy under **Agents & access → Connected apps**.

## What data it sends

- The plugin contains no code. It points Claude at the MarketsEasy server `https://api.marketseasy.com/mcp`; sign-in happens at `https://auth.marketseasy.com`.
- Claude sends MarketsEasy the requests it makes for you: searches, order and product ids, and the fields of any change it proposes. If you ask it to create an order, the customer name and delivery address you give it are sent to MarketsEasy and wait for your approval.
- MarketsEasy answers with data your account may see. Order results leave out customer names, addresses and phone numbers; they show the order's country, status, tracking and carrier.
- The plugin stores nothing. MarketsEasy keeps a log of each agent request and approval, which you can review under **Agents & access → Activity**.

Privacy policy: https://marketseasy.com/privacy · Terms: https://marketseasy.com/terms · Support: contact@marketseasy.com
