# -goit-react-hw-06-redux

1. npx create-react-app . --use-npm
2. npm i prop-types
3. линтинг npm install --save-dev prettier husky lint-staged
4. Проверяем настройки VSCode(autoSeve - onFocusChange; formatOnSave - вкл;
   codeActionsOnSave - all)
5. Добавляем настройки в
   проект(https://github.com/goitacademy/react-lint-config)
6. настраиваем абсолютные импорты
   (https://create-react-app.dev/docs/importing-a-component/#absolute-imports)
   (создаем файл jsconfig.json,вставляем... после чего можно писать import
   Button from 'components/Button'; без ../../../)
7. Ставим пакет [https://reactrouter.com/core/guides/quick-start] - (npm install
   react-router-dom)
8. Анимированная стилизация npm install react-transition-group
9. Redux - npm i redux
10. React-redux - npm i react-redux
11. Redux DevTools (http://extension.remotedev.io/) - npm install --save-dev
    redux-devtools-extension
12. В файл с редьюсером import { createStore, applyMiddleware } from 'redux';
    import { composeWithDevTools } from 'redux-devtools-extension'; const store
    = createStore(reducer, composeWithDevTools());
13. Redux Toolkit - npm install @reduxjs/toolkit
14. logger [https://github.com/LogRocket/redux-logger] - показывает все actions
    красиво в консоле

15. deploy on netlify
16. В корне создать файл netlify.toml - ( [build] publish = "build"

    [[redirects]] from = "/" to = "/index.html" status = 200)

17. npm install netlify-cli -g
18. netlify login
19. Authorized
20. package.json ("predeploy": "npm run build", "deploy": "netlify deploy -p")
21. npm run deploy
22. Create (enter), enter, name project
23. netlify open --site

24. 0.12 Coздаем store, папку redux
25. 0.17 Объявляем actions
26. 0.27 На примере Counter создаем в actions increment & decrement
27. 0.30 Пишем под них reducer
28. 0.36 Соединяем все файлы с помощью пакета react-redux. ReduxProvider
29. 0.42 Передаем пропсами state в Counter (mapStateToProps)
30. 0.46 Передаем методы для отправки actions (mapDispatchToProps)
31. 0.53 Переписываем в store весь initialState и соответсвенно весь файл
32. 1.02 Redux DevTools
33. Композиция редюсеров - import { combineReducers } from 'redux';
34. Разбиваем отдельно на редьюсеры весь стейт 24 1.17 Рефакторим код
35. 1.24 Переписываем todos, todos-types.js
36. 1.28 todos-reducer.js
37. 1.30 store.js
38. 1.31 todos-actions.js
39. 1.37 TodoEditor.js

40. Вебинар 10 Redux Toolkit
41. Redux Toolkit
42. 0.03 ConfigureStore()
43. 0.06 Оставляем DevTools только для разработки (devTools:
    process.env.NODE_ENV === 'development')
44. 0.08 Сокращаем rootReducer
45. 0.10 Ставим logger [https://github.com/LogRocket/redux-logger]
46. 0.14 createAction()
47. 0.08 Prepare Callback - используем при сложном payload
48. 0.22 createReducer()
49. 0.26 файл todos-types.js больше не нужен
50. 0.34 Пишем toggleCompleted
51. 0.28 component Stats
52. 0.43 Закрываем модалку при сохранении тудушки
53. 0.46 redux-persist [https://github.com/rt2zz/redux-persist] npm install
    redux-persist
54. 0.52 Исправляем index.js ({PersistGate})
