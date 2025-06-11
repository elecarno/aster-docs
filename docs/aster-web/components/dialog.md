---
title: Dialog
layout: default
has_toc: true
parent: Components
---

```css
.pan-bg-darken {
    height: 100%;
    width: 100%;
    
    position: fixed;
    top: 0;
    left: 0;
    z-index: 2 !important;
    
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    
    background-color: rgba(0, 0, 0, 0.5);
}

#gra-dialog-logo {
    width: 360px;
    margin-bottom: 128px;
}

.pan-dialog {
    width: clamp(250px, var(--prefwidth), 85%);
    
    position: absolute;
    
    display: grid;
    
    padding: 10px;
    
    background-color: var(--panel-2);
    
    border-bottom: 3px solid var(--panel-3);
    border-radius: var(--radius-3);;
}

.con-dialog-content {
    max-height: 80vh;
    width: 100%;
    overflow-y: auto;
    
    display: flex;
    flex-direction: column;
    justify-content: center;
    row-gap: 5px;
}

.lab-dialog-title {
    margin-bottom: 10px; 
    margin-left: auto; 
    margin-right: auto; 
    margin-top: 4px;
    
    font-size: 18px;
    text-align: center
}

.con-dialog-buttons {
    height: 36px;
    
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    column-gap: 5px;
    
    padding-top: 14px;
}

.btn-dialog-exit {
    height: 100%;
    width: 100%;
    
    font-size: var(--font-size-body);
}
```