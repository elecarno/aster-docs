---
title: PanelServerView
layout: default
has_toc: true
parent: Components
---

```css
.con-server-area {
    width: 100%;

    float: right;

    display: flex;
    flex-direction: row;
    justify-content: stretch;

    margin-bottom: 25px;

    border-bottom-left-radius: var(--radius-2);

    overflow: hidden;
}

.con-message-area {
    height: calc(100% - 48px);

    display: flex;
    flex-direction: column-reverse;

    margin-left: 10px;
    margin-right: 10px;

    overflow: hidden;
    overflow-y: scroll
}

.pan-server-messages {
    height: 100%;
    
    float: right;

    display: flex;
    flex-direction: column;
    flex: 1;

    background-color: var(--panel-2);

    border-left: 3px var(--panel-0) solid;

    box-sizing: border-box;
    overflow: hidden;
}
.pan-server-channels {
    width: 240px;

    display: flex;
    flex-direction: column;

    color: var(--text-gray);
    background-color: var(--panel-2);
}

.con-channel-toggle {
    display: flex;
    flex-direction: row;

    margin-left: 8px;
    margin-bottom: 4px;
}
.con-channel-toggle span {
    width: 80%;
    text-align: center;
}

.con-message-input {
    width: calc(100% - 32px);

    display: flex;
    flex-direction: row;

    margin: 16px;
    margin-bottom: 20px;
}

@media (max-width: 1024px) {
    .con-server-area {
        margin-bottom: 0;
        border-radius: 0;
    }

    .pan-server-channels {
        width: 100%;
    }

    .pan-server-messages {
        border: none;
    }

    .con-message-input {
        margin: 8px;
    }

    .inp-message {
        margin: 0px;
    }
}

.inp-message {
    max-height: 128px;
    width: 100%;
    
    padding-top: 12px;
    padding-left: 24px;
    padding-right: 24px;
    
    color: #d3d3d3;
    background: var(--panel-1);
    
    border-radius: var(--radius-2);

    font-size: var(--font-size-body);
}
.inp-message:focus {
    outline: 0;
}

.con-server-info {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: left;
}
.lab-server-ip {
    margin-bottom: 15px;
    margin-left: auto;
    margin-right: auto;
}
.lab-server-info {
    margin: 0;
    margin-left: 10%;
    
    font-size: 13px;
}

.btn-server-profile {
    width: 80%;
    
    margin: 0 auto;
    margin-top: 10px;
    margin-bottom: 14px;
    
    padding: 5px;
    
    font-size: 14px;
}
```