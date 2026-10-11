---
exo__Asset_uid: 9df9ffac-af6c-4d45-a8f3-a8b820b13df3
exo__Asset_createdAt: 2026-10-12T03:34:56
exo__Asset_updatedAt: 2026-10-12T03:34:56
exo__Instance_class:
  - "[[9a1cf31c-9d41-4ef3-9023-584a8d087d16]]"
exo__Asset_createdBy: "[[4ef3962d-b8a7-42b5-bd28-88ec846f1d13]]"
exo__Asset_label: skos__closeMatch
aliases:
  - skos__closeMatch
exo__Asset_isDefinedBy: "[[87873ce4-d071-48aa-a422-fe6ace301316]]"
exo__Property_cardinality: "[[59a37aa7-ffbe-4e0d-ba60-06ae370d880f]]"
exo__Property_domain: "[[493c2ae2-de56-47ec-954d-2eb8cb49bff7]]"
exo__Property_range: "[[ebc65c03-1417-48e5-930a-48f41478c9fb]]"
exo__Slugable_slug: closeMatch
exo__Property_displayName: closeMatch
---

# skos__closeMatch

Стандартное свойство соответствия W3C SKOS <http://www.w3.org/2004/02/skos/core#closeMatch>: понятия достаточно близки, чтобы иногда взаимозаменять их, но не во всех задачах.

- **Где применяется:** утверждения соответствия «стола» сравнения авторов (`$desk-mappings`) — `exo__Statement` [понятие автора, `skos__closeMatch`, нейтральное понятие стола]. Предикат в утверждении — **голым UID** этого ассета, не ссылкой по имени (RFC `14217015` §CQ4, AC8; шаг стола скилла `exoize-source` отвергает ссылку по имени до записи).
- **Пример:** «Ум» автора ↔ «Мышление» стола.
- **domain:** `exo__Asset` · **range:** `skos__Concept` · кратность — множественная. Решение по мандату фаундера 2026-10-11 23:18 (фаундер вправе пересмотреть): range узкий — CLI SHACL проверяет его через утверждение адаптера стола `concept__Concept ⊂ skos__Concept`; domain широкий — иначе без того же ребра субъект не проверялся бы вовсе (находка ревью PR kitelev/exocortex#4558).
- **Вывод SKOS** (симметричность, транзитивность, обратность) движок не делает — запросы стола на нём не строятся.

Источник: RFC `14217015-963b-4020-b267-fd13b1275b3a` §5; лист `6d3d7dd2-e379-4d2d-b655-080df7cba88e`.

