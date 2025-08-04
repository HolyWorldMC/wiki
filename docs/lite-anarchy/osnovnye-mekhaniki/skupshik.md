# Скупщик

**Скупщик** — это система продажи предметов за внутриигровую валюту (монеты) и очки скупщика. Система включает множительные коэффициенты, которые увеличиваются в зависимости от объема и ценности проданных товаров.

## Доступ к системе

Скупщик доступен через команду `/b` или `/buyer`, а также через NPC на спавне. Для автоматической продажи предметов используется команда `/buyer auto`.

За продажу предметов игроки получают:
- **Монеты** — основная игровая валюта
- **Очки скупщика** — используются для покупок в магазине скупщика и увеличения коэффициента

<img src="/docs/lite-anarchy/osnovnye-mekhaniki/assets/magazin.png" alt="Демонстрация магазина скупщика и очков" width="75%">

## Система множителей

### Глобальный множитель
Глобальный множитель повышается за получение очков скупщика:
- Базовое повышение: +<!-- wiki[buyer-global-multiplier-base] -->0.01<!-- /wiki -->× за каждые <!-- wiki[buyer-global-multiplier-points] -->N<!-- /wiki --> очков
- Для обладателей Stinger+: +<!-- wiki[buyer-global-multiplier-premium] -->0.02<!-- /wiki -->× за каждые <!-- wiki[buyer-global-multiplier-points] -->N<!-- /wiki --> очков

### Повышение цены на товары

**Инвестиции**
Через систему `/invest` можно улучшать "Товар скупщика". После каждого улучшения случайный товар получает +<!-- wiki[invest-buyer-bonus] -->10<!-- /wiki -->% к цене. Бонус суммируется, если один товар выпадает несколько раз.

**Временные усиления**
- **Бустер скупщика** — доступен в `/shop`
- **Ульта скупщика** — повышает цену всех товаров на <!-- wiki[buyer-ultra-bonus] -->10<!-- /wiki -->% в течение <!-- wiki[buyer-ultra-duration] -->1 часа<!-- /wiki -->

### Формирование цен
Цены на товары сбрасываются три раза в день в случайное время. При сбросе цены не обнуляются полностью, а корректируются по специальной формуле.

## Категории принимаемых товаров

### Шахтные ресурсы
Максимальный множитель для этой категории составляет ×<!-- wiki[buyer-mining-max-multiplier] -->1.1<!-- /wiki -->.

| Ресурс | Базовая цена (монеты) |
|--------|----------------------|
| Уголь | <!-- wiki[buyer-price-coal] -->2<!-- /wiki --> |
| Лазурит | <!-- wiki[buyer-price-lapis] -->3<!-- /wiki --> |
| Редстоун | <!-- wiki[buyer-price-redstone] -->3<!-- /wiki --> |
| Эндерняк | <!-- wiki[buyer-price-endstone] -->3<!-- /wiki --> |
| Кварц | <!-- wiki[buyer-price-quartz] -->25<!-- /wiki --> |
| Железный слиток | <!-- wiki[buyer-price-iron] -->40<!-- /wiki --> |
| Золотой слиток | <!-- wiki[buyer-price-gold] -->50<!-- /wiki --> |
| Обсидиан | <!-- wiki[buyer-price-obsidian] -->100<!-- /wiki --> |
| Алмаз | <!-- wiki[buyer-price-diamond] -->150<!-- /wiki --> |
| Древний обломок | <!-- wiki[buyer-price-debris] -->950<!-- /wiki --> |
| Изумруд | <!-- wiki[buyer-price-emerald] -->1000<!-- /wiki --> |
| Незеритовый лом | <!-- wiki[buyer-price-netherite-scrap] -->1000<!-- /wiki --> |
| Незеритовый слиток | <!-- wiki[buyer-price-netherite-ingot] -->4200<!-- /wiki --> |

### Материалы с мобов
Максимальный множитель достигает ×<!-- wiki[buyer-mob-max-multiplier] -->1.25<!-- /wiki -->.

| Материал | Базовая цена (монеты) |
|----------|----------------------|
| Гнилая плоть | <!-- wiki[buyer-price-flesh] -->1<!-- /wiki --> |
| Стрела | <!-- wiki[buyer-price-arrow] -->1.5<!-- /wiki --> |
| Кости | <!-- wiki[buyer-price-bone] -->1.5<!-- /wiki --> |
| Нитки | <!-- wiki[buyer-price-string] -->2<!-- /wiki --> |
| Паучий глаз | <!-- wiki[buyer-price-spider-eye] -->4<!-- /wiki --> |
| Стержень ифрита | <!-- wiki[buyer-price-blaze-rod] -->10<!-- /wiki --> |
| Слизь | <!-- wiki[buyer-price-slime] -->20<!-- /wiki --> |
| Сгусток магмы | <!-- wiki[buyer-price-magma-cream] -->25<!-- /wiki --> |
| Шерсть | <!-- wiki[buyer-price-wool] -->25<!-- /wiki --> |
| Кожа | <!-- wiki[buyer-price-leather] -->40<!-- /wiki --> |
| Жареная баранина | <!-- wiki[buyer-price-cooked-mutton] -->40<!-- /wiki --> |
| Жареная свинина | <!-- wiki[buyer-price-cooked-pork] -->40<!-- /wiki --> |
| Эндер-жемчуг | <!-- wiki[buyer-price-ender-pearl] -->50<!-- /wiki --> |
| Череп визер-скелета | <!-- wiki[buyer-price-wither-skull] -->100<!-- /wiki --> |
| Маринованный паучий глаз | <!-- wiki[buyer-price-fermented-spider-eye] -->125<!-- /wiki --> |
| Порох | <!-- wiki[buyer-price-gunpowder] -->125<!-- /wiki --> |
| Светокаменная пыль | <!-- wiki[buyer-price-glowstone] -->250<!-- /wiki --> |
| Слеза гаста | <!-- wiki[buyer-price-ghast-tear] -->750<!-- /wiki --> |

### Древесные материалы
Максимальный множитель ×<!-- wiki[buyer-wood-max-multiplier] -->1.5<!-- /wiki -->.

| Тип древесины | Базовая цена (монеты) |
|---------------|----------------------|
| Ель | <!-- wiki[buyer-price-spruce] -->30<!-- /wiki --> |
| Темный дуб | <!-- wiki[buyer-price-dark-oak] -->30<!-- /wiki --> |
| Дуб | <!-- wiki[buyer-price-oak] -->40<!-- /wiki --> |
| Береза | <!-- wiki[buyer-price-birch] -->40<!-- /wiki --> |
| Акация | <!-- wiki[buyer-price-acacia] -->40<!-- /wiki --> |
| Багровый стебель | <!-- wiki[buyer-price-crimson] -->60<!-- /wiki --> |
| Искажённый стебель | <!-- wiki[buyer-price-warped] -->60<!-- /wiki --> |

### Зелья
Максимальный множитель ×<!-- wiki[buyer-potion-max-multiplier] -->1.5<!-- /wiki -->.

| Тип зелья | Базовая цена (монеты) |
|-----------|----------------------|
| Силы II | <!-- wiki[buyer-price-strength] -->225<!-- /wiki --> |
| Скорости II | <!-- wiki[buyer-price-speed] -->230<!-- /wiki --> |
| Огнестойкость | <!-- wiki[buyer-price-fire-resistance] -->330<!-- /wiki --> |
| Невидимость | <!-- wiki[buyer-price-invisibility] -->400<!-- /wiki --> |

### Сельскохозяйственная продукция
Максимальный множитель ×<!-- wiki[buyer-farming-max-multiplier] -->1.25<!-- /wiki -->.

| Культура | Базовая цена (монеты) |
|----------|----------------------|
| Нарост | <!-- wiki[buyer-price-wart] -->4<!-- /wiki --> |
| Сладкие ягоды | <!-- wiki[buyer-price-berries] -->5<!-- /wiki --> |
| Морковь | <!-- wiki[buyer-price-carrot] -->5<!-- /wiki --> |
| Картофель | <!-- wiki[buyer-price-potato] -->6<!-- /wiki --> |
| Ломтик арбуза | <!-- wiki[buyer-price-melon-slice] -->10<!-- /wiki --> |
| Бамбук | <!-- wiki[buyer-price-bamboo] -->10<!-- /wiki --> |
| Ламинария | <!-- wiki[buyer-price-kelp] -->10<!-- /wiki --> |
| Какао-бобы | <!-- wiki[buyer-price-cocoa] -->12<!-- /wiki --> |
| Пшеница | <!-- wiki[buyer-price-wheat] -->20<!-- /wiki --> |
| Свекла | <!-- wiki[buyer-price-beetroot] -->20<!-- /wiki --> |
| Плод хоруса | <!-- wiki[buyer-price-chorus] -->24<!-- /wiki --> |
| Тростник | <!-- wiki[buyer-price-sugarcane] -->80<!-- /wiki --> |
| Арбуз | <!-- wiki[buyer-price-melon] -->80<!-- /wiki --> |
| Тыква | <!-- wiki[buyer-price-pumpkin] -->80<!-- /wiki --> |
| Кактус | <!-- wiki[buyer-price-cactus] -->125<!-- /wiki --> |

## Магазин скупщика

Через команду `/buyer shop` игроки могут тратить накопленные очки скупщика. Стоимость товаров увеличивается после каждой покупки.

| Товар | Цена (очки) | Особенности |
|-------|-------------|-------------|
| **Ульта Скупщика** | <!-- wiki[buyer-shop-ultra-price] -->100<!-- /wiki --> | +<!-- wiki[buyer-ultra-bonus] -->10<!-- /wiki -->% монет с продажи на 1 час |
| **Бустер очков Скупщика** | <!-- wiki[buyer-shop-booster-price] -->150<!-- /wiki --> | +<!-- wiki[buyer-booster-bonus] -->20<!-- /wiki -->% очков на 1 час |
| **Бустер Культур** | <!-- wiki[buyer-shop-crops-price] -->200<!-- /wiki --> | +<!-- wiki[buyer-crops-bonus] -->25<!-- /wiki -->% выпадения растений на 1 час |
| **Опыт** | <!-- wiki[buyer-shop-exp-price] -->250<!-- /wiki --> | <!-- wiki[buyer-shop-exp-amount] -->1000<!-- /wiki --> уровней |
| **Жетон на титул** | <!-- wiki[buyer-shop-title-price] -->500<!-- /wiki --> | Один раз за вайп |
| **Донат-кейс** | <!-- wiki[buyer-shop-donate-price] -->750<!-- /wiki --> | Один раз за вайп |
| **Зачарованное золотое яблоко** | <!-- wiki[buyer-shop-golden-apple-price] -->100<!-- /wiki --> | — |
| **Рассадник** | <!-- wiki[buyer-shop-spawner-price] -->300<!-- /wiki --> | — |
| **Особый компас** | <!-- wiki[buyer-shop-compass-price] -->400<!-- /wiki --> | — |
| **Загадочное яйцо призыва** | <!-- wiki[buyer-shop-egg-price] -->350<!-- /wiki --> | — |
| **Элитры** | <!-- wiki[buyer-shop-elytra-price] -->450<!-- /wiki --> | — |
| **Взрывная трапка** | <!-- wiki[buyer-shop-trap-price] -->200<!-- /wiki --> | — |
| **Осколочное яйцо** | <!-- wiki[buyer-shop-shard-egg-price] -->180<!-- /wiki --> | — |
| **Золотая кирка Джейка** | <!-- wiki[buyer-shop-jack-pickaxe-price] -->320<!-- /wiki --> | — |
| **Книга зачарования "Фермер II"** | <!-- wiki[buyer-shop-farmer-book-price] -->280<!-- /wiki --> | — |
