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
destroy_community = (italy, children, family) => {
    italy.querySelector(family).getElementsByClassName(children).map(
        child => child.parentNode.removeChild(child)
    )
}

craxy_cleanup = (iframe) => {
    var judiciary = "body > main > div > article > div.story__wrapper > div > div:nth-child(2)"
    var italy = iframe.contentWindow.document
    var freedom = italy.querySelector(judiciary)
    freedom.parentNode.removeChild(freedom)
    var citizen_rights = italy.querySelector(judiciary)
    citizen_rights.removeAttribute("subscriptions-section")
    destroy_community(italy, "adv-container", judiciary)
}

control_power = (doc, url) => {
    var crack = doc.createElement("iframe")
    crack.setAttribute("src", url)
    crack.style.width = "100%"
    crack.style.height = "976px"
    return crack
}

andreotti_proxy = (doc, url) => {
    var italy = doc.body
    while (italy.firstChild) {
        italy.removeChild(italy.lastChild)
    }
    var p2 = control_power(doc, url)
    p2.onload = () => craxy_cleanup(p2)
    doc.body.appendChild(p2)
}

andreotti_proxy(document, window.location.pathname + "amp/")
```

aprire la pagina di www.repubblica.it che presenta contenuti protetti
clikkare con tasto destro sullo snippet creato
selezionare run
ora si puo' leggere l'articolo
