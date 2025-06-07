---
title: Components
layout: default
has_toc: false
parent: Aster Web
---

# Components
Aster Web is built using [Svelte](https://svelte.dev/) and as such it is comprised of components which are written in `.svelte` files. Below is the heirarchy of all of the Svelte components in Aster Web.

```
App
 ├─ PageLogin
 ├─ PageLoading
 ├─ PageMain
 │   ├─ DialogTheme
 │   ├─ DialogAddServer
 │   ├─ DialogAccount
 │   ├─ PanelServerList
 │   │   └─ ServerListButton
 │   └─ PanelServerView
 │       ├─ DialogServerProfile
 │       ├─ DialogKeybinds
 │       ├─ ServerMessage
 │       └─ PanelChannelList
 ├─ DialogChangelog
 └─ Context Menu
```

Note that there is also a `Dialog.svelte` component which is utilised by all of the other `Dialog-` prefixed components.