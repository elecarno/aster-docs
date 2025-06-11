---
title: PageMain
layout: default
has_toc: true
parent: Components
---

```css
.con-main {
    height: 100%; 
    width: 100%;
    
    display: flex;
    flex-direction: row;
}

@media (width >= 1024px) {
    .con-sidebar {
        height: 100%;
        width: 200px;
        min-width: 200px;
    }

    .con-top-buttons {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;

        margin-top: 20px;
        margin-bottom: 10px;
    }

    .btn-addserver,
    .btn-aster,
    .btn-account {
        margin-left: 6px;
    }
}

@media (width < 1024px) {
    .con-sidebar {
        height: 100%;
        width: 70px;
        min-width: 70px;
    }

    .con-top-buttons {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;

        margin-top: 20px;
        margin-bottom: 16px;
    }

    .btn-addserver,
    .btn-aster {
        margin-bottom: 5px;
        margin-left: 0px;
    }
    .btn-account {
        margin-left: 0px;
    }
}

.con-channel-edge-separator {
    height: 100%;
    min-width: 18px
}

.btn-addserver,
.btn-account,
.btn-aster {
    height: 46px;
    width: 46px;

    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;

    margin-top: 0;

    color: var(--white-1);
    background-color: var(--panel-2);

    border-style: none;
    border-radius: var(--radius-2);

    transition: background-color 0.4s ease;
}

.btn-aster {
    background-color: var(--accent-1-light);
}
.btn-aster:hover {
    background-color: var(--panel-2);
}
.btn-aster:hover path {
    stroke: var(--accent-1-light);
}

#gra-main-logo path{
    transition: stroke 0.4s ease;
}

.con-main-bg-logo {Add commentMore actions
    height: 100%;
    width: 100%;

    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
}
#gra-main-bg-logo {
    height: 40%;
    width: 40%;

    margin-bottom: 5%;
}

.btn-addserver:hover,
.btn-account:hover {
    background-color: var(--panel-1);
}
```