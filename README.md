# Smeta Mini App — GitHub Pages

Это статическое мини-приложение для ведения сметы, адаптированное под iPhone и публикацию через GitHub Pages.

## Что внутри

- `index.html` — само приложение
- `.nojekyll` — отключает Jekyll на GitHub Pages

## Как загрузить в GitHub

### Вариант 1 — через сайт GitHub
1. Создай новый репозиторий, например `smeta-app`
2. Нажми **Add file** → **Upload files**
3. Загрузи `index.html`, `README.md` и `.nojekyll`
4. Нажми **Commit changes**

### Вариант 2 — через git локально
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/USERNAME/smeta-app.git
git push -u origin main
```

## Как включить GitHub Pages
1. Зайди в репозиторий на GitHub
2. Открой **Settings** → **Pages**
3. В блоке **Build and deployment** выбери:
   - **Source** → `Deploy from a branch`
   - **Branch** → `main`
   - **Folder** → `/ (root)`
4. Нажми **Save**
5. Подожди 1–3 минуты

После этого приложение будет доступно по адресу:

```text
https://USERNAME.github.io/smeta-app/
```

## Как открыть на iPhone
1. Открой ссылку GitHub Pages в Safari
2. Нажми **Поделиться**
3. Выбери **На экран «Домой»**

## Важно
- Все данные сохраняются в `localStorage` браузера
- Данные привязаны к конкретному Safari и конкретному устройству
- Если открыть приложение на другом iPhone, база будет пустой
- Если очистить данные Safari, записи удалятся

## Что уже работает
- Проекты
- Добавление записей
- Графики
- Аналитика
- Календарь
- Экспорт CSV
- Свайп-удаление
- Тёмная и светлая тема
