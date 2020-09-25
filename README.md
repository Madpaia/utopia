# utopia
Utopia: a truly free repubblica 

aggiungete il codice seguente come nuovo snippet in chrome.

aprire chrome
 - dev tools (Command+Option+I)
 - tab Sources
 - sub tab Snippets
 - '+ New Snippet'
sul frame a destra incollate lo script:
```
ANDREOTTI = document.querySelector("body news-app").root.querySelector("iron-pages news-article").root.querySelector("div.container div.content amp-viewer div.amp-doc-host").shadowRoot.querySelector("body main article div.detail-article_container div.detail-article_body section");
ANDREOTTI && ANDREOTTI.parentNode.removeChild(ANDREOTTI);
document.querySelector("body news-app").root.querySelector("iron-pages news-article").root.querySelector("div.container div.content amp-viewer div.amp-doc-host").shadowRoot.querySelector("body main article div.detail-article_container div.detail-article_body div[subscriptions-section='content']").removeAttribute("subscriptions-section");
```

aprire la pagina di repubblica coni contenuti protetti
clikkare con tasto destro sullo snippet creato
selezionare run
ora si puo' leggere l'articolo
