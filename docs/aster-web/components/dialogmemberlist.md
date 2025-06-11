---
title: DialogMemberList
layout: default
has_toc: true
parent: Components
---

```css
.con-memberlist-scrollbox {
    min-height: 400px;
    max-height: 600px;
    width: 95%;

    margin: 0 auto;
    
    overflow-y: scroll;
}
.con-memberlist-member {
    display: flex;
    flex-direction: row;
    justify-content: left;
    align-items: center;
    column-gap: 16px;

    margin-bottom: 10px;

    border-radius: var(--radius-3);
}
.con-memberlist-member:hover {
    background-color: var(--panel-3);
}

.gra-memberlist-pfp {
    height: 32px;
    width: 32px;

    border-radius: 50%;
}

.lab-memberlist-displayname {
    margin: 0;
}
```