
<h1 align="center">
  <br>
  <a href="https://stratumprotocol.org"><img src="https://github.com/stratum-mining/stratumprotocol.org/blob/660ecc6ccd2eca82d0895cef939f4670adc6d1f4/src/.vuepress/public/assets/stratum-logo%402x.png" alt="SRI" width="200"></a>
  <br>
Stratum V2 Reference Implementation (SRI)
  <br>
</h1>

<h4 align="center">SRI is a refference implementation of the Stratum V2 protocol written in Rust 🦀.</h4>

<p align="center">
  <a href="https://codecov.io/gh/stratum-mining/stratum">
    <img src="https://codecov.io/gh/stratum-mining/stratum/branch/main/graph/badge.svg" alt="codecov">
  </a>
  <a href="https://twitter.com/intent/follow?screen_name=stratumv2">
    <img src="https://img.shields.io/twitter/follow/stratumv2?style=social" alt="X (formerly Twitter) Follow">
  </a>
</p>

## 💼 Table of Contents

<p align="center">
  <a href="#introduction">Introduction</a> •
  <a href="#getting-started">Getting Started</a> •
  <a href="#use-cases">Use Cases</a> •
  <a href="#roadmap">Roadmap</a> •
  <a href="#contribute">Contribute</a> •
  <a href="#support">Support</a> •
  <a href="#supporters">Supporters</a> •
  <a href="#donate">Donate</a> •
  <a href="#donate">License</a> •
</p>

## 👋Introduction

Welcome to the official GitHub repository for the SRI - Stratum V2 Reference Implementation. [Stratum V2](https://stratumprotocol.org) is a next-generation bitcoin mining protocol designed to enhance the efficiency, security, flexibility and decentralization. 

SRI is fully open-source, community-developed, independent of any single entity, aiming to be fully compatible with [Stratum V2 Specification](https://github.com/stratum-mining/sv2-spec).

## ⛏️Getting Started

To get started with the Stratum V2 Reference Implementation (SRI), please follow the detailed setup instructions available on the official website:

[Getting Started with Stratum V2](https://stratumprotocol.org/getting-started/)

This guide provides all the necessary information on prerequisites, installation, and configuration to help you begin using, testing or contributing to SRI.

## 🚀 Use Cases

The library is modular to address different use-cases and desired functionality. Examples include:

### 👷Miners

- Sv1 Miners can use the translator proxy (`roles/translator`) to connect with a Sv2-compatible pool.
- Sv1 mining farms mining to a Sv2-compatible pool gain some of the security and efficiency improvements Sv2 offers over Stratum V1 (Sv1). The Sv1<->Sv2 translator proxy does not support  _all_ the features of Sv2, but works as a temporary measure before upgrading completely to Sv2-compatible firmware. (The Sv1<->Sv2 translation proxy implementation is a work in progress.)

### 🛠️Pools

- Pools supporting Sv2 can deploy the open source binary crate (`roles/pool`) to offer their clients (miners participating in said pool) an Sv2-compatible pool.
- The Rust helper library provides a suite of tools for mining pools to build custom Sv2 compatible pool implementations.
- The C library provides a set of FFI bindings to the Rust helper library for miners to integrate Sv2 into their existing firmware stack.

## 🛣Roadmap 

Our roadmap is publicly available, outlining current and future plans. Decisions on the roadmap are made through a consensus-driven approach, through participation on dev meetings, Discord or GitHub.

[View the SRI Roadmap](https://github.com/orgs/stratum-mining/projects/5)

### 🎯Goals

The goals of this project are to provide:

1. A robust set of Stratum V2 (Sv2) primitives as Rust library crates which anyone can use
   to expand the protocol or implement a role. For example:
   - Pools supporting Sv2
   - Mining-device/hashrate producers integrating Sv2 into their firmware
   - Bitcoin nodes implementing Template Provider to build the `blocktemplate`
2. The above Rust primitives as a C library available for use in other languages via FFI.
3. A set of helpers built on top of the above primitives and the external Bitcoin-related Rust crates for anyone to implement the Sv2 roles.
4. An open-source implementation of a Sv2 proxy for miners.
5. An open-source implementation of a Sv2 pool for mining pool operators.

## 💻Contribute 

If you are a developer looking to help, but you're not sure where to begin, check the [good first issue label](https://github.com/stratum-mining/stratum/labels/good%20first%20issue), which contains small pieces of work that have been specifically flagged as being friendly to new contributors.

Contributors looking to do something a bit more challenging, before opening a pull request, please join [our community chat](https://chat.btcpayserver.org/) or [start a GitHub discussion](https://github.com/btcpayserver/btcpayserver/discussions) to get early feedback, discuss the best ways to tackle the problem, and ensure there is no work duplication and consensus.

## 🤝Support

Join our Discord community to get help, share your ideas, or discuss anything related to Stratum V2 and its refference implementation. 

Whether you're looking for technical support, want to contribute, or are just interested in learning more about the project, our community is the place to be.

[Join the Stratum V2 Discord Community](https://discord.gg/fsEW23wFYs)

## 🎁Donate

### 👤Individual Donations 
If you wish to support the development and maintenance of the Stratum V2 Reference Implementation, individual donations are greatly appreciated. You can donate through OpenSats, a 501(c)(3) public charity dedicated to supporting open-source Bitcoin projects.

[Donate through OpenSats]()

### 🏢Corporate Donations
For corporate entities interested in providing more substantial support, such as grants to SRI contributors, please get in touch with us directly. Your support can make a significant difference in accelerating development, research, and innovation.

Email us at: stratumv2@gmail.com

## 📖License
This software is licensed under Apache 2.0 or MIT, at your option.

---

> Website[stratumprotocol.org](https://www.stratumprotocol.org) &nbsp;&middot;&nbsp;
> Discord [SV2 Discord](https://discord.gg/fsEW23wFYs) &nbsp;&middot;&nbsp;
> Twitter [@Stratumv2](https://twitter.com/StratumV2)
