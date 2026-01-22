<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/authrim/.github/main/assets/logo-dark.svg" width="280">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/authrim/.github/main/assets/logo-light.svg" width="280">
  <img alt="Authrim" src="https://raw.githubusercontent.com/authrim/.github/main/assets/logo-light.svg" width="280">
</picture>

### Open Source Identity & Access Platform for the modern web

[![Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/authrim/authrim/blob/main/LICENSE)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?logo=typescript)](https://www.typescriptlang.org/)
[![Cloudflare Workers](https://img.shields.io/badge/Cloudflare-Workers-orange?logo=cloudflare)](https://workers.cloudflare.com/)

<br>

[Website](https://authrim.com) · [Documentation](https://authrim.com/getting-started/introduction/) · [Get Started](#get-started)

</div>

---

## What is Authrim?

**Authrim** is a serverless Identity Hub that combines authentication, authorization, and identity federation — all running on **Cloudflare's global edge network** with **<50ms latency worldwide**.

<table>
<tr>
<td width="50%" valign="top">

### ✅ OpenID Certified

<a href="https://openid.net/certification/">
  <img src="https://raw.githubusercontent.com/authrim/authrim/main/docs/images/openid-certified.jpg" alt="OpenID Certified" height="80">
</a>

Certified by the [OpenID Foundation](https://openid.net/certification/):

- **7 OpenID Provider profiles**
- **4 Logout profiles**

</td>
<td width="50%" valign="top">

### ⚡ One Command Setup

Deploy your own identity platform in minutes:

```bash
npx @authrim/setup
```

[Setup documentation →](https://github.com/authrim/authrim/tree/main/packages/setup)

</td>
</tr>
</table>

---

## Features

| Authentication | Authorization | Identity Hub |
|:--------------|:--------------|:-------------|
| Passkey / WebAuthn | RBAC / ABAC / ReBAC | Social Login (7+ providers) |
| Email OTP | Real-time Check API | Identity Linking |
| SAML 2.0 IdP/SP | Policy Engine | PII/Non-PII Separation |
| Device Flow | WebSocket Push | SCIM 2.0 Provisioning |

**Plus:** OAuth 2.0 / OIDC compliant, PAR, DPoP, JAR, JARM, OpenID4VP/VCI, and more.

---

## Get Started

### Quick Start

```bash
# Interactive setup wizard
npx @authrim/setup
```

### SDKs

| Package | Description | |
|---------|-------------|---|
| [`@authrim/web`](https://github.com/authrim/js-web) | Browser SDK with Passkey, Social Login, Email Code | [![npm](https://img.shields.io/npm/v/@authrim/web?color=blue)](https://www.npmjs.com/package/@authrim/web) |
| [`@authrim/core`](https://github.com/authrim/js-core) | Platform-agnostic OIDC client | [![npm](https://img.shields.io/npm/v/@authrim/core?color=blue)](https://www.npmjs.com/package/@authrim/core) |

```javascript
import { createAuthrim } from '@authrim/web';

const auth = await createAuthrim({
  issuer: 'https://your-tenant.authrim.com',
  clientId: 'your-client-id',
});

// Passkey login
await auth.passkey.login();
```

---

## Repositories

| Repository | Description |
|------------|-------------|
| [**authrim/authrim**](https://github.com/authrim/authrim) | Core identity platform (Cloudflare Workers) |
| [**authrim/js-web**](https://github.com/authrim/js-web) | Browser SDK (`@authrim/web`) |
| [**authrim/js-core**](https://github.com/authrim/js-core) | Core SDK (`@authrim/core`) |
| [**authrim/example-web**](https://github.com/authrim/example-web) | Vanilla JS example app |

---

<div align="center">

**[Documentation](https://docs.authrim.com)** · **[Dashboard](https://dashboard.authrim.com)** · **[GitHub](https://github.com/authrim/authrim)**

<sub>Apache 2.0 License · Built with ❤️ on Cloudflare Workers</sub>

</div>
