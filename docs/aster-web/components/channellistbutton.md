---
title: ChannelListButton
layout: default
has_toc: true
parent: Components
---

```css
.btn-channel {
    min-height: 30px;
    width: 96%;
    
    padding-left: 20px;
    
    color: var(--text-gray);
    background-color: inherit;
    
    border: none;
    border-radius: var(--radius-3);
    
    font-size: var(--font-size-body);
    text-align: left;
    
    box-sizing: border-box;
    list-style-type: none;
}
.btn-channel:hover {
    background-color: var(--panel-1);
}

button:global(.btn-channel[value="1"]) {
    background-color: var(--panel-3);
}
```