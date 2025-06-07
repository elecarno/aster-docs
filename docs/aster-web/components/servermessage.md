---
title: ServerMessage
layout: default
has_toc: true
parent: Components
---

```css
.con-message-image {
    display: flex;
    flex-direction: column;
}

.gra-message-image {
    max-height: 512px;
    max-width: 60%;
    width: min-content;
    
    object-fit: contain;
}

.con-message {
    display: flex;
    flex-direction: row;
    align-items: stretch;
    justify-content: stretch;
    
    margin-top: var(--spacing);
    
    padding-left: 8px;
    
    color: var(--text-gray);
    
    border-radius: var(--radius-3);
}
.con-message:hover {
    background-color: var(--panel-3);
}

.lab-message-username {
    min-width: var(--uname-width);
    
    margin: 0;
    margin-top: var(--uname-top);
    margin-left: 10px;
    margin-right: 6px;
    
    font-size: var(--font-size-body);
}

.lab-message-username-mobile {
    margin: 0;
    margin-top: var(--uname-top);
    margin-left: 10px;
    
    color: var(--text-gray);
    
    font-size: var(--font-size-body);
}

.lab-message-date {
    min-width: 130px;

    margin: 0;
    margin-top: var(--date-top);
    margin-left: auto;
    margin-right: 15px;
    
    font-family: var(--font-body-mono);
    font-size: 10px;
    text-align: right;
}

.lab-message-date-mobile {
    margin: 0;
    margin-top: var(--date-top);
    
    color: var(--text-gray);
    
    font-family: var(--font-body-mono);
    font-size: 10px;
}

.gra-message-pfp {
    height: 24px;
    width: 24px;
    
    margin: 0;
    
    border-style: none;
    border-radius: 50%;
    
    background-position: center;
    object-fit: cover;
}

.con-message-body {
    max-width: 100%;
    
    margin: 0;
    margin-top: var(--body-top);
    margin-left: 2px;
    
    color: var(--white-1);
    
    white-space: pre-line;
}
```