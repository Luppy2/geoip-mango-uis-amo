# geoip-mango-uis-amo

Кастомный `geoip.dat` в формате V2Ray для клиента **HAPP** (и любого Xray/sing-box).
Содержит категории: `ru`, `private`, `mango`, `uis`, `amocrm`.

Собирается автоматически компилятором [v2fly/geoip](https://github.com/v2fly/geoip)
из актуальных данных RIPE каждую неделю (и при ручном запуске).

## Прямая ссылка на файл (для поля `Geoipurl` в HAPP)

```
https://github.com/Luppy2/geoip-mango-uis-amo/releases/download/latest/geoip.dat
```

## Категории

| Категория | Источник (ASN) | Что покрывает |
|---|---|---|
| `ru` | v2fly | весь российский IP-трафик |
| `private` | v2fly | локальные сети |
| `mango` | AS39684 Mango Telecom | телефония Mango Office (SIP, ЛК, API) |
| `uis` | AS34832 NovoSystem | телефония UIS / uiscom |
| `amocrm` | AS39134 UnitedNet | сервисы amoCRM (API, drive, edge) |

## Как обновить вручную

Actions → «Build Custom V2Ray GeoIP» → Run workflow. Через ~2–3 минуты
релиз `latest` обновится новым файлом по той же ссылке.

Списки-fallback лежат в `sources/` на случай недоступности RIPE.
