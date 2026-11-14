# HTB Writeups

Разборы лабораторных машин Hack The Box: последовательность исследования, результаты, ограничения доказательств и выводы для защиты.

Автор: [d7n98jhk52-debug](https://github.com/d7n98jhk52-debug) · [Профиль HTB](https://app.hackthebox.com/public/users/4100352)

| Машина | ОС | Сложность по снимку HTB | Основные темы | Результат |
|---|---|---|---|---|
| [Bedside](writeups/bedside.md) | Linux | Medium | PDF/CMap, pickle, Path Traversal, SSH, MONAI checkpoint | User и Root owned |
| [DanglingTree](writeups/danglingtree.md) | Windows | Medium | WAC, сервисные credentials, DPAPI, AD ACL, AD CS | User и Root owned |
| [BlockSynergy](writeups/blocksynergy.md) | Linux (Ubuntu 24.04 по отчёту) | Не указана | VIP, SSRF, Ping Node, Smart Contract, FTP, backup/restore | User принят по отчёту; root не подтверждён |

## Как читать

Каждый разбор содержит последовательность действий, результат, ограничения доказательств и меры защиты. Скриншоты HTB подтверждают принятие обоих флагов для Bedside и DanglingTree. Для BlockSynergy принятие User Flag отражено по тексту предоставленного отчёта; root не получен, TOCTOU остаётся гипотезой.

Значения флагов, пароли, приватные ключи, сертификаты с закрытыми ключами и Kerberos-билеты не публикуются.

Материалы относятся к лаборатории HTB. Названия пользователей, доменов и внутренние адреса в технических иллюстрациях относятся к стенду. Это описания конкретных исследований, а не заявление об обнаружении новых уязвимостей в продуктах.

## Структура

- `writeups/` — три райтапа на русском языке.
- `assets/` — иллюстрации и подтверждения результата.
- `reports/` — [предоставленный PDF по BlockSynergy](reports/BlockSynergy_HTB_RU.pdf).

Рабочие артефакты эксплуатации не включены. В райтапах отдельно обозначено, какие детали не подтверждены исходными доказательствами.
