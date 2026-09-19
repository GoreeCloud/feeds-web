# GoreeCloud Feeds Web Specifications

## Status

Component: GoreeCloud Feeds Web  
Repository: GoreeCloud/feeds-web  
Component class: Web application  
Lifecycle: Planned  
Implementation status: Repository documentation foundation only

This specification scopes the web-client responsibilities derived from the governing GoreeCloud Feeds product roadmap. It does not establish implementation.

## Authority boundary

GoreeCloud Feeds Web is intended to present and manage authorized GoreeCloud Feeds state while GoreeCloud Feeds Server remains authoritative for server-owned feed ingestion, processing, search, storage, synchronization, and administration state.

The web client must not silently create an incompatible second authority for server-owned data.

## Planned interface capabilities

- Home dashboard and Today view.
- Feed navigation and article lists.
- Clean article reader.
- Unread management.
- Saved articles and favorites.
- Reading history.
- Reading-position synchronization.
- Search.
- Folders and tags.
- Smart Feeds.
- Rules management.
- Settings.
- Feed-health presentation.
- Offline interface where safe and practical.
- Explicit connection and synchronization state.
- Notification-related settings/presentation where supported.
- Authorized administration interface.
- Responsive desktop/tablet/mobile presentation.
- Keyboard and touch-friendly interaction.
- Accessibility and reduced-motion/transparency behavior.
- Current Official Stable Glaze UI adoption.

## Protocol boundary

Client/server communication should use versioned shared contracts owned by GoreeCloud/feeds-protocol. The web client should not depend on undocumented server internals.

## Offline boundary

Offline behavior should preserve local usability and user changes where supported without silently overwriting server-authoritative state. Synchronization failures and conflicts must remain visible and recoverable.

## Privacy and security

The client should minimize unnecessary external requests, avoid advertising/profiling dependencies, protect session and account state, and avoid leaking article/feed content through diagnostics.

## Open decisions

No web framework, programming language, package manager, bundler, offline-storage engine, service-worker design, test framework, browser support matrix, deployment host, authentication implementation, or API transport is selected by this foundation.
