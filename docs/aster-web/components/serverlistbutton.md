---
title: ServerListButton
layout: default
has_toc: true
parent: Components
---

```css
.con-btn-server {
    width: 100%;
    height: fit-content;
}

@media (width >= 1024px) {
    .btn-server {
        width: calc(100% - 20px);
        
        margin: 10px;
        
        padding: 10px;
        padding-left: 13px;
        
        background-color: var(--panel-2);
        
        border-radius: var(--radius-2);
        
        box-sizing: border-box;
    }
    .btn-server:hover {
        background-color: var(--panel-1);
    }

    .con-server-name {
        display: flex;
        flex-direction: row;
        align-items: center;
    }
    .lab-server-name {
        margin: 0;
        margin-left: 10px;
        
        font-size: 18px;
        text-align: left;
    }
    .gra-server-icon {
        height: 48px;
        width: 48px;
        
        border-radius: var(--radius-2);
        
        box-sizing: content-box;
    }

    .lab-server-tagline {
        margin: 0;
        margin-top: 5px;
    }

    button:global(.btn-server[value="0"]) {
        padding-left: 13px;
        border: none;
    }
    button:global(.btn-server[value="1"]) {
        padding-left: 10px;
        border-left: 3px solid var(--accent-1-light);
    }
}

@media (width < 1024px) {
    .btn-server {
        height: 57px;
        width: 57px;
        
        margin-bottom: 5px;
        margin-left: 5px;
        
        background-color: var(--panel-2);
        
        border-radius: var(--radius-2);
        
        box-sizing: border-box;
    }

    .con-server-name {
        display: flex;
        flex-direction: row;
        align-items: center;
    }
    .lab-server-name {
        display: none;
    }
    .gra-server-icon {
        height: 48px;
        width: 48px;
        
        border-radius: calc(var(--radius-2) - 4px);
        
        box-sizing: content-box;
    }

    .lab-server-tagline {
        display: none;
    }
}
```