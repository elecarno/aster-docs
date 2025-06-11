---
title: ContextMenu
layout: default
has_toc: true
parent: Components
---

```css
* {
    margin: 0;
    padding: 0;

    font-size: 13px;
}

.pan-conmenu {
    width: 250px;
    
    display: inline-flex;
    flex-direction: column;
    
    padding-top: 5px;
    padding-bottom: 5px;
    padding-right: 5px;
    
    background-color: var(--panel-2);
    
    border: 1px var(--panel-3) solid;
    border-radius: var(--radius-2);
    
    overflow: hidden;
    filter: drop-shadow(0px 5px 7px var(--panel-1));
}
.pan-conmenu ul{
    margin: 6px;
}

ul li{
    width: 1fr;
    display: block;
    list-style-type: none;
}
ul li button{
    height: 28px;
    width: 100%;
    
    color: var(--white-1);
    background-color: var(--panel-2);
    
    border: 0px;
    
    text-align: left;
}
ul li button:hover{
    color: var(--text-gray);
    background-color: var(--panel-3);
    
    border-radius: var(--radius-3);
    
    text-align: left;
}
ul li button i{
    padding: 0px 15px 0px 10px;
}

hr{
    width: 100%;
    margin: 5px 0px;
}

.lab-conmenu-shortcut {
    float: right;
    color: var(--text-gray);
}
```