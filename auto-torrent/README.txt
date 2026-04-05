# Автоматизация скачивания фильмов и сериалов

Референсные мануалы:
1. https://connect.smartliving.ru/profile/225/blog/ustanovka-i-nastroyka-sonarr-radarr-qbittorrent-jackett-torproxy-v-docker.html
2. https://habr.com/ru/articles/719572/

### Проект автоматического поиска и скачивания сериалов и фильмов с последующей их публикацией в медиосервисе PLEX. 
Стек:
- qbittorrent
- jackett - индексер/индексатор торрентов
- sonarr + radarr - можно сказать ядро системы, в их вебморде происходит подача запроса на скачивание, они отдают команду индексеру, а в последствии qbittorent и plex.
- plex
- wireguard - если находитесь в стране, со всевозможными банами и ошраничениями интернета
Железо, NAS terramaster f2-425, 8GB RAM. TOS6.0, в случае если у вас увеличенный объем ОЗУ, либо вам хвататие дефолтных 4GB, и у вас не очень быстрые диски, рекомендую выключать swap, инчате при нескольких активных закгрузках, система может быть менее отзывчивой.

---

# Automated downloading of movies and TV series

Reference manuals:
1. https://connect.smartliving.ru/profile/225/blog/ustanovka-i-nastroyka-sonarr-radarr-qbittorrent-jackett-torproxy-v-docker.html
2. https://habr.com/ru/articles/719572/

### A project for automatically searching and downloading TV series and movies, followed by their publication on the PLEX media service.

Stack:
- qbittorrent
- jackett - torrent indexer
- sonarr + radarr - the core of the system, so to speak. Their web interface processes download requests, which they then send to the indexer, and subsequently to qbittorrent and plex.
- plex
- wireguard - if you're in a country with all sorts of internet bans and restrictions
Hardware: Terramaster f2-425 NAS, 8GB RAM. TOS 6.0. If you have more RAM, or the default 4GB is enough for you, and your drives aren't very fast, I recommend disabling swap. Inchat may be less responsive during multiple active downloads.
