---
title: "Nodes Silently Miss Events"
url: "https://docs.envio.dev/blog/nodes-silently-miss-events"
date: "2026-09-07"
feed_url: "https://docs.envio.dev/blog/rss.xml"
---
Execution clients sometimes drop logs from eth_getLogs, and a JSON-RPC response does not show whether it is complete. This article documents some of the cases, explains which parts of an EVM block can be checked against the header's Merkle roots, and describes how HyperSync recomputes transaction and receipt roots on every ingested block.
