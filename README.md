# Химия для будущего архитектора — v3

Добавлено:
- бесплатные видео без обязательной подписки InternetUrok;
- `progress.html` — личная страница ученицы;
- `parent.html` — родительская статистика;
- Supabase Auth + RLS для безопасной синхронизации;
- в облако уходят только статусы уроков, факт открытия видео и мини-тесты;
- заметки, рисунки и цифровой планшет остаются локально.

## Подключение Supabase
1. Создать Supabase project.
2. Выполнить `supabase-setup.sql` в SQL Editor.
3. В Authentication → URL Configuration добавить Site URL `https://savenkovawb-maker.github.io/chemistry-for-architect/` и redirect URLs для `progress.html` и `parent.html`.
4. В `supabase-config.js` записать Project URL и Publishable key (или legacy anon key). НИКОГДА не использовать service_role/secret key.
5. Commit/push в `main`; GitHub Pages обновится.
