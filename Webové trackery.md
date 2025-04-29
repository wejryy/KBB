### Cookies
- HTTP Cookies - malé textové soubory uložené v prohlížeči, které obsahují unikátní ID uživatele
- Trvalé cookies - zůstávají uloženy i po zavření prohlížeče 
- Third-party cookies - ukládají se z domén třetích stran (google ads, facebook pixel,...)

### Pixelové tagy (Tracking pixels)
- malé (1x1px) neviditelné obrázky načítané ze serveru trackeru
- při načtení stránky se odešle HTTP požadavek na tracker včetně informací (IP,user-agent, čas na stránce,..)


### Local storage & Session storage
- moderní alternativa k cookies, která umožňuje ukládat větší množství dat
- některé trackery (např. analytické nástroje) zde ukládají identifikátory uživatelů

### Fingerprinting
- kombinace různých parametrů prohlížeče (user-agent, rozlišení, časové pásmo,fonty,pluginy,..) vytvoří unikátní "otisk"
- i při blokování cookies lze uživatele stále identifikovat 

### Supercookies
- pokročilé trackery využívají více uložišť (flash cookies, HTML5 localStorage, IndexedDB) k obnovení ID i po smazání klasických cookies


### Referrery (HTTP hlavičká Referer)
- při kliknutí na odkaz, prohlížeč odešle původní URL v hlavičče Referer
- trackery tak mohou sledovat, odkud uživatel přišel

### CNAME Cloaking (Maskování trackerů)
- některé trackery se maskují jako subdomény hlavního webu(např. tracker.seznam.cz), aby obešly blokování třetích stran

### Webové analytické nástroje
- Google Analytics, Matomo, Hotjar -> sledují chování uživatelů pomocí JavaScriptu
- nahrávají scrollování, klikání, čas strávený na stránce

### Reklamní sítě (AdTech)
- Google Ads, Facebook Pixel -> sdílejí data mezi weby, aby cílovaly reklamy
- umožňují retargeting(např. "sledování" produktů, které jste prohlíželi na jiném webu)

### Jak se bránit?
Blokování trackerů :
				 - rozšíření jako uBlock Origin, Privacy Badger, Ghostery
				 - prohlížeče s ochranou proti sledování (Brave, Firefox,...)
Vypnutí třetích cookies v nastavení prohlížeče
VPN / Tor -> skrytí IP adresy
DuckDuckGO / Startpage -> vyhledávače, které nesledují