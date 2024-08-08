# Grafana Dashboard for Cloudflare Firewall Events

## Overview

This repository contains a minimalist Grafana dashboard designed to visualize `firewallEventsAdaptive` data from the Cloudflare GraphQL endpoint. The dashboard utilizes the Infinity data source plugin to retrieve and display Cloudflare firewall events.

**Note:** This dashboard is compatible with free Cloudflare accounts, but the data retrieval time range is limited to a maximum of 24 hours.

## Getting Started

### Step 1: Generate an API Key

To enable the Infinity data source to authenticate with Cloudflare, you need to generate a bearer token. Follow these steps:

1. Log in to your Cloudflare account.
2. Navigate to **My Profile** under your account settings.
3. Select **API Tokens** and click on **Create Token**.
4. Choose the "Read analytics and logs" template.
5. Generate the token and save it securely.

### Step 2: Configure the Data Source

1. In Grafana, add a new Infinity data source.
2. In the data source settings, enter your Cloudflare bearer token.
3. Add the Cloudflare endpoint as allowed host: `https://api.cloudflare.com/client/v4/graphql`.

### Step 3: Configure the Dashboard

1. Import the provided dashboard JSON file into Grafana.
2. In the dashboard settings, configure it to use the Infinity data source.
3. Enter your Cloudflare Account ID (which you can find in your Cloudflare Dashboard) and assign a custom name for the account.

## Contributing

Contributions and extensions to this dashboard are welcome! If you add new features, please ensure they are compatible with Cloudflare Free accounts, or isolate them in a separate section of the dashboard.

For questions, feedback, or further information, feel free to reach out at [fourframes.de](https://fourframes.de).
