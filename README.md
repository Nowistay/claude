# Nowistay

Run your vacation rental business from a conversation with Claude. The Nowistay plugin connects Claude to your [Nowistay](https://www.nowistay.com) account so you can check bookings, availability and prices, read and answer guest messages, plan cleaning and maintenance missions, edit welcome guides, and maintain the private knowledge your AI co-host uses, without switching tools.

## What you can ask

- "What needs my attention today across my properties?"
- "Raise the nightly rate by 10% on Fridays and Saturdays in July for The Beauty Villa."
- "Show me the last messages from the guest arriving tomorrow and draft a reply."
- "Create a direct booking for 12 to 15 August and send a payment link."
- "Who is assigned to next week's cleanings?"
- "Update the Wi-Fi password in the welcome guide."
- "Build a CSV of last month's revenue and cleaning costs by property."

## Skills

| Skill | What it does |
| --- | --- |
| `daily-brief` | Arrivals, departures, urgent missions and guest conversations that need a decision |
| `calendar-revenue` | Review and update availability, nightly rates, stay rules and restrictions |
| `direct-bookings` | Create or update direct bookings, with optional payment links |
| `guest-messaging` | Find conversations, summarize them, draft and send replies |
| `guest-records` | Find returning guests and add guests to your customer base |
| `team-operations` | Plan, assign and follow up cleaning, maintenance and custom missions |
| `welcome-guide` | Create and edit welcome guide pages, translations and images |
| `property-knowledge` | Maintain and copy the private Q&A your AI co-host answers from |
| `portfolio-reporting` | Revenue, fees, commissions, cleaning costs and workload reports across properties |

## Requirements

- A Nowistay account. Sign up at [nowistay.com](https://www.nowistay.com).
- Properties with the AI co-host feature and an active Nowistay PMS connection. Other properties are not visible to Claude.

## Connect

1. Install the plugin, then open its **Connectors** tab and connect **Nowistay**.
2. Sign in with your Nowistay account and approve the requested access.
3. Ask Claude about your properties.

In Claude Code, the plugin connects to the same server and asks you to sign in the first time a Nowistay tool runs.

## How changes are applied

Every change goes through two steps. Claude first stages the change with a preview tool and shows you exactly what will happen. Nothing is written until you confirm and Claude calls the matching confirm tool with the one-time approval token from that preview. Read-only questions never change your data.

## Data

The plugin itself contains only instructions (skills) and a reference to the Nowistay MCP server at `https://api.nowistay.com/mcp`. It runs no local code and stores nothing on your machine.

When you use it, Claude sends your requests to that server over HTTPS using an OAuth token scoped to your Nowistay account. The server returns property, calendar, booking, mission, guest, message, welcome guide and knowledge base data for your eligible properties only. Guest contact details and private notes are omitted by default and returned only when you explicitly ask for them. Nowistay does not send your data to any other destination through this plugin.

See the [Nowistay privacy policy](https://www.nowistay.com/privacy) and [terms of use](https://www.nowistay.com/terms-of-use).

## Support

Contact us at [nowistay.com/contact-us](https://www.nowistay.com/contact-us).
