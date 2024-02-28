# Playwright (TS binding) + Cucumber (BDD)


## Sample report
![image](https://github.com/ortoniKC/Playwright_Cucumber_TS/assets/58769833/da2d9f5a-85e7-4695-8ce2-3378b692afc4)


## Project structure

- .github -> yml-файл для выполнения тестов в GitHub Actions
- src -> Содержит все функции и код TypeScript
- test-results -> Содержит все файлы, связанные с отчетами

## Reports

1. [Отчет Mutilple Cucumber](https://github.com/WasiqB/multiple-cucumber-html-reporter)
2. Стандартный отчет Cucumber
3. [Логи](https://www.npmjs.com/package/winston)
4. Скриншоты неудач
5. Тестовые видео неудач
6. Трассировка неудач

## Get Started

### Установка:

1. Клонировать или скачать проект
2. Извлечь и открыть в VS-Code
3. `npm i` для установки зависимостей
4. `npx playwright install` для установки браузеров
5. `npm run test` для выполнения тестов
6. Для запуска конкретного теста изменить
```
  paths: [
            "src/test/features/featurename.feature"
         ] 
```
7. Использовать теги для запуска конкретного или группы спецификаций
```
npm run test --TAGS="@test or @add"
```

### Folder structure
0. `src/pages` -> Все страницы (экраны UI)
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

