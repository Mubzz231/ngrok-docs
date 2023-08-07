---
sidebar_position: 1
title: Overview
---

# Agent SDKs

---

## Overview

Agent SDKs enable you to embed ngrok directly into your application. They allow
you to programmatically create ngrok endpoints. You handle connections from
ngrok's edge just as if you opened a socket to listen on a port.

## Languages

| Language   | Docs                                                       | Quickstart                                      | Repository                                                             | Status |
| ---------- | ---------------------------------------------------------- | ----------------------------------------------- | ---------------------------------------------------------------------- | ------ |
| Go         | [ngrok-go Docs](https://pkg.go.dev/golang.ngrok.com/ngrok) | [ngrok-go quickstart](/getting-started/go/)     | [github.com/ngrok/ngrok-go](https://github.com/ngrok/ngrok-go)         | Stable |
| Rust       | [ngrok-rust Docs](https://docs.rs/ngrok/latest/ngrok/)     | [ngrok-rust quickstart](/getting-started/rust/) | [github.com/ngrok/ngrok-rust](https://github.com/ngrok/ngrok-rust)     | Stable |
| Python     | [ngrok-python Docs](https://ngrok.github.io/ngrok-python/) |                                                 | [github.com/ngrok/ngrok-python](https://github.com/ngrok/ngrok-python) | Beta   |
| JavaScript | [ngrok-nodejs Docs](https://ngrok.github.io/ngrok-nodejs/) |                                                 | [github.com/ngrok/ngrok-nodejs](https://github.com/ngrok/ngrok-nodejs) | Beta   |
| Java       |                                                            |                                                 | [github.com/ngrok/ngrok-java](https://github.com/ngrok/ngrok-java)     | Alpha  |

## When are Agent SDKs a good choice?

Agent SDKs are often a better fit for your use case over using the [ngrok
agent](/agent/). This is especially true when running ngrok with
production apps. Agent SDKs are a better choice if:

- You don't want to manage the lifetime of a separate agent process
- You don't to bundle and distribute the ngrok agent
- The ngrok agent doesn't run on your target platform
- The ngrok agent's resource requirements are too high for your target platform
- You want fine-grained programmatic control over the agent's functionality

## Pricing

The agent SDKs are available to all ngrok users at no additional charge. You
only incur costs if the resources provisioned by the SDKs incur a cost.
