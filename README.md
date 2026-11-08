# Yandex Wordstat MCP by MCPKit

**English** · [Русский](README_RU.md)

Research Yandex search demand, discover keyword ideas and explore seasonality from ChatGPT. A hosted Model Context Protocol (MCP) service for SEO specialists, PPC marketers, content teams and business owners working with Yandex search audiences.

**MCPKit is currently free to use. Three MCP tools with command details loaded on demand. No coding or local server setup.**

**Yandex Search API statistics requests are billed separately by Yandex through your own Yandex Cloud account.**

**[Sign up for MCPKit](https://mcpkit.ru/mcp-wordstat)** — choose **Регистрация** (Register) on the website.  
[Get an API key](https://mcpkit.ru/instructions/wordstat/api-key) · [Connect ChatGPT](https://mcpkit.ru/instructions/wordstat/chatgpt)

This repository contains product information and usage examples for the cloud service. Server source code is not distributed here.

## Turn search demand into a research starting point

Find what people search for, explore related queries, compare regions and identify seasonal patterns. Use the returned data to discuss keyword groups, advertising ideas or website content with your AI.

- **Popular queries:** get phrases containing your seed terms and their search counts.
- **Related queries:** explore associations returned separately from the popular-query list.
- **Demand over time:** request daily, weekly or monthly dynamics for supported periods.
- **Regional demand:** compare regions or cities by count, share and affinity index.
- **Device filters:** research demand on desktop, phone or tablet where supported.
- **Your own connection:** save your Yandex Search API key and Folder ID in the dashboard and select the active account.

Four data commands support these workflows: popular queries, dynamics, regional distribution and a region directory. Grouping keywords or drafting a content plan is work the AI performs using those results, not a separate clustering feature of the server.

## Three tools, details on demand

MCPKit exposes just three MCP tools: `tool_list`, `tool_help`, and `tool_execute`. Your AI can request the command catalog, load the detailed instructions for the command it needs, then run it.

The full schemas for every command are not included in the initial tool definitions. This keeps the initial context footprint small, including when you are discussing something else. Catalogs, help and results still use tokens when requested; actual savings depend on the AI client and conversation.


## Try these requests in ChatGPT

These are example prompts, not customer results. Russian seed phrases below target Russian-language demand; keep the seed phrase in the language of the audience you want to research.

| Your task | Example prompt |
| --- | --- |
| Initial keyword research | “Find popular queries containing ‘ремонт квартир’ in Moscow.” |
| Discover adjacent topics | “Show related queries for ‘купить диван’ and suggest additional topics to investigate.” |
| Advertising groups | “Get queries for ‘доставка цветов’ in Moscow, then propose ad groups based on the returned phrases.” |
| SEO page planning | “Get queries for ‘кухни на заказ’ and suggest groups for separate website pages.” |
| Seasonal planning | “Show monthly demand for ‘кондиционеры’ over the available completed period and identify seasonal peaks.” |
| Regional opportunities | “Compare cities for ‘тепловой насос’. Show search counts and affinity index before suggesting where to investigate further.” |

For a campaign brief, start with a seed phrase, narrow the region and devices, then ask the AI to organize the returned queries. Researching additional seed phrases requires additional API calls.

## Connect without programming

1. [Register or sign in to MCPKit](https://mcpkit.ru/mcp-wordstat). One account works with all three services.
2. Follow the [Yandex Cloud setup guide](https://mcpkit.ru/instructions/wordstat/api-key) to obtain your API key and Folder ID with the required access and billing setup.
3. Save them in the [Wordstat dashboard](https://mcpkit.ru/mcp-wordstat/panel) and select the active account. Enter keys in the dashboard, not in your AI chat.
4. Copy the server URL. Add a custom MCP connection in ChatGPT, choose **OAuth**, sign in to MCPKit and authorize access.
5. Select the connection and ask: **“Show the available Wordstat commands.”** Then try a keyword query from the table above.

**MCP server URL:** `https://mcpkit.ru/mcp-wordstat/mcp`

You need an AI client/account that supports adding remote MCP servers with OAuth. ChatGPT is the primary documented client; other compatible clients may require different setup.

[Illustrated ChatGPT connection guide](https://mcpkit.ru/instructions/wordstat/chatgpt) (Russian). The API-key guide is also in Russian.

## Availability, costs and limits

MCPKit access is currently free, as stated on the [service website](https://mcpkit.ru/mcp-wordstat). Yandex bills statistics requests separately; any AI-client subscription is also separate. Check current Yandex Cloud terms when setting up billing.

Each data command accepts one seed phrase. Popular-query results support up to 2,000 phrases; this is not an exhaustive export of all keywords. Popular queries and regional distribution cover the last 30 days. Historical availability and operators depend on the selected dynamics period and Yandex rules.

Search counts measure demand, not unique buyers or sales. Overlapping keyword counts should not be added as unique audience size. The service does not provide search rankings or guaranteed advertising costs. Paid requests are not automatically retried by the server.
## One MCPKit account, three services

Register once to use all three cloud services. Each has its own settings and a separate MCP connection:

| Service | What you can do |
| --- | --- |
| [Yandex Direct](https://mcpkit.ru/mcp-yandex-direct) | Analyze advertising and manage campaigns |
| [Yandex Metrica](https://mcpkit.ru/mcp-yandex-metrika) | Explore website traffic and conversions |
| [Yandex Wordstat](https://mcpkit.ru/mcp-wordstat) | Research keywords, demand and seasonality |

Explore demand with Wordstat, work on advertising with Direct, and assess website performance with Metrica. Connect the services you need; this is not an automatic cross-service workflow.

**[Start researching Yandex search demand with MCPKit](https://mcpkit.ru/mcp-wordstat)**

