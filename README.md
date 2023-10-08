# `did:webhash` Decentralized Identifiers Method Spec

This repository contains the `did:webhash` Decentralized Identifier Method Specification. You can access the latest version of this specification here:

https://did.coop/did-method-webhash/

The W3C Community Group that is works on the specification of which this is a fork can be found here:

https://w3c-ccg.github.io/did-method-web/

## Editing and building the specification

This specification uses [ReSpec](https://github.com/w3c/respec/) html. Just edit `index.html` and the draft will be rendered correctly.

When it's time to do a static snapshot, we use the ReSpec UI in the browser to export static HTML.

## Design Goals & Use Cases Overview:

- signed DID documents
  - JCS canonicalization support --> proof format to allow either DI or JOSE-based verification tooling
- content-addressed URLs for each DID document over time (incl. static hosting)
- optional/backwards-compatible extensions for:
  - historical queries via ?versionTime= and ?versionId=
  - backwards compatibility (deterministic translation from did:webhash URI --> did:web URI, redirect and/or dual-static hosting for did:web-based systems)
  - witnessing mechanisms: trusted caching clients, historical sync, etc.

For a more detailed overview of design process, use-cases and goals, see:
- https://github.com/WebOfTrustInfo/rwot12-cologne/blob/main/advance-readings/did-web-2.0.md
- https://github.com/w3c-ccg/did-method-web/issues?q=is%3Aissue+