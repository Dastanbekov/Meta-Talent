# Meta Talent · Frontend MVP

Адаптивный демо-интерфейс для хакатона: тест профориентации, персональные роадмапы, клубы из Бишкеке/онлайн и мини-чат с ИИ на мок-данных. Собран на React + Tailwind + Framer Motion (mobile-first) и комплектуется Storybook для показа ключевых компонентов.

## Требования окружения

- Node.js ≥ 20.19 (используем через `nvm`)
- npm ≥ 10

## Скрипты

| Команда | Назначение |
| --- | --- |
| `npm run dev` | локальный дев-сервер Vite (http://localhost:5173) |
| `npm run build` | production-бандл + проверка TypeScript |
| `npm run preview` | предпросмотр собранной версии |
| `npm run storybook` | Storybook с примерами UI (порт 6006) |
| `npm run build-storybook` | статическая сборка Storybook |

## Что внутри

- **Landing** с AI-хиро, live-счётчиком пользователей, отзывами и блоком под командный матчинг.
- **Test Wizard** на 6 вопросов с описанием вариантов, распределением топ-ролей и CTA в роадмап.
- **Roadmap**: свайпер карточек + модалки с ресурсами, чек-листы со стейком в LocalStorage, AI Coach Tips.
- **Insights**: персональные инсайты, Meta Talent Card, action deck, события, testimonials и 팀-виджет.
- **Clubs & Events**: фильтры по формату/тегам, карта с маркерами, таймлайн событий и “резерв места”.
- **AI Co-Pilot**: сценарии (“Подготовка к хакатону” и др.), typing-индикатор и контекстные советы.
- **Storybook** истории для `GradientButton`, `Navbar`, `ChatWidget`, `InsightStatCard`, `CoachTipCard`, `MapFilters`.
- Мок-данные в `src/data/mockContent.ts`, типы — `src/types/content.ts`.

## Дизайн / UX штрихи

- Tailwind-токены (`brand.*`, градиенты, стекло-эффекты) в `tailwind.config.js`.
- Framer Motion: анимации карточек, слайдеры, модалки, number-ticker.
- Сохранение прогресса роадмапа в LocalStorage, AI tips, карта с интерактивными маркерами.
- Компонентная структура (`src/components/*`, `src/sections/*`) готова под Storybook и дальнейшее масштабирование.

## Как показать на демо

1. **Run app**: `npm run dev`, показать `/`, `/test`, `/roadmap`, `/insights`, `/clubs`.
2. **Storybook**: `npm run storybook` для каталогизации UI и дизайн-системы.
3. **Build**: `npm run build` для прод-демо или деплоя (Vercel/Netlify).

Feel free to обновлять мок-данные, стили и анимации прямо в соответствующих файлах — структура уже готова под быстрые итерации.
# Meta-Talent
