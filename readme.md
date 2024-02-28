# Playwright (TS) + Cucumber (BDD)

## Структура проекта

- .github -> yml-файл для выполнения тестов в GitHub Actions
- src -> Содержит все функции и код TypeScript
- test-results -> Содержит все файлы, связанные с отчетами

## Отчеты

1. [Отчет Mutilple Cucumber](https://github.com/WasiqB/multiple-cucumber-html-reporter)
2. Стандартный отчет Cucumber
3. [Логи](https://www.npmjs.com/package/winston)
4. Скриншоты неудач
5. Тестовые видео неудач
6. Трассировка неудач


## Старт

### Установка:

1. `npm i` для установки зависимостей
2. `npx playwright install` для установки браузеров
3. `npm run test` для выполнения тестов
4. Для запуска конкретного теста изменить
```
  paths: [
            "src/test/features/featurename.feature"
         ] 
```
5. Использовать теги для запуска конкретного или группы спецификаций
```
npm run test --TAGS="@test or @add"
```

### Структура папок
0. `src/pages` -> Все страницы 
1. `src/test/features` -> здесь пишите ваши функции
2. `src/test/steps` -> Здесь находятся ваши определения шагов
3. `src/hooks/hooks.ts` -> Логика настройки и завершения работы браузера
4. `src/hooks/pageFixture.ts` -> Простой способ делиться объектами страниц с шагами
5. `src/helper/env` -> Управление несколькими средами
6. `src/helper/types` -> Для получения подсказок кода среды
7. `src/helper/report` -> Для генерации отчета
8. `config/cucumber.js` -> Один файл для всей магии
9. `package.json` -> Содержит все зависимости
10. `src/helper/auth` -> Состояние хранения (Auth файл)
11. `src/helper/util` -> Чтение тестовых данных из json и логгер

