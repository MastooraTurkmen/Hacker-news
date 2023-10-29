# HackerNews

> Awareness about the _Hacker News_

> https://wonderful-hacker-news.netlify.app/

Quick start:

```
$ npm install
$ npm start
```

Head over to https://vitejs.dev/ to learn more about using vite

## Screenshotes of HackerNews

1. Top
2. New
3. Ask
4. Show
5. Favorites

### _1 Top_

![Alt text](Screenshot-1.png)

### _2 New_

![Alt text](Screenshot-2.png)

### _3 Ask_

![Alt text](Screenshot-3.png)

### _4 Show_

![Alt text](Screenshot-4.png)

### _5 Favorites_

![Alt text](Screenshot-5.png)

## _App JS_

```
    import RouterHandler from "./router.js";

    window.onhashchange = () => {
    setActiveLink();
    };

    function setActiveLink() {
    const links = document.querySelectorAll(".header-link");
    links.forEach((link) => {
        const linkPath = link.getAttribute("href");
        const currentPath = window.location.hash;
        if (currentPath === linkPath) {
        link.classList.add("active");
        } else {
        link.classList.remove("active");
        }
    });
    }

    class App {
    constructor() {
        new RouterHandler();
    }
    }

    new App();


```
