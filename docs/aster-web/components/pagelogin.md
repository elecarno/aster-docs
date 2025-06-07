---
title: PageLogin
layout: default
has_toc: true
parent: Components
---

```css
.con-login {
    width: 40%;
    min-width: 350px;
    max-width: 500px;

    position: absolute;
    transform: translate(-50%, -50%);
    left: 50%;
    top: 50%;

    display: flex;
    flex-direction: column;

    padding: 10px;

    border-radius: var(--radius-3);
}
.pan-login {
    display: flex;
    flex-direction: column;
    align-items: stretch;
    justify-content: center;

    padding: 15px;

    color: var(--white-1);
    background-color: var(--panel-2);

    border-bottom: 3px solid var(--panel-3);
    border-radius: var(--radius-2);
}

#gra-login-logo {
    width: 360px;
    margin: 0 auto;
    padding-bottom: 32px;
}

.con-login-input {
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-direction: row;

    margin-top: 8px;
    margin-bottom: 8px;
}
.con-login-input p {
    width: 30%;
    margin: 0;
    font-size: var(--font-size-body);
}

.inp-login {
    height: 45px;
    width: 70%;

    color: var(--white-1);
    margin-left: 8px;

    font-size: var(--font-size-body);
    text-align: center;
}

.btn-login {
    height: 40px;
    width: 80%;

    color: var(--text-dark);
    background-color: var(--accent-1-light);

    font-size: var(--font-size-body);
}
.btn-login:hover {
    background-color: var(--accent-1-dark);
}

.lab-splash-text {
    height: 100px;
    
    display: flex; 
    flex-direction: column; 
    align-items: center; 
    justify-content: center;

    font-size: 18px;
    text-align: center;
    
    transition: 0.5s ease;

    -webkit-user-select: none;
    -ms-user-select: none;
    user-select: none;
}
.lab-splash-text:hover {
    font-size: 18.5px;
}
```