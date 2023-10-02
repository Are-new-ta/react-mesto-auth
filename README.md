<h1 align="center">Учебный frontend-проект: "Место"</h1>

<div align="center">
    <img src="https://user-images.githubusercontent.com/108838349/215305563-5d7a1891-fdbd-4142-b011-6ece3ec74cee.gif" width="550" alt="Гиф с демонстрацией функционала приложения">
 </div>

<a name="summary">
  <details>
    <summary>Оглавление</summary>
    <ol>
      <li><a href="#project-description">Описание проекта</a></li>
      <li><a href="#technologies">Стек технологий</a></li>
      <li><a href="#installation">Установка и запуск приложения в локальном репозитории, эксплуатация</a></li>
      <li><a href="#establishing">Процесс создания</a></li>
      <li><a href="#functionality">Функционал</a></li>
        </ol>
  </details>
</a>

<a name="project-description"><h2>1. Описание проекта</h2></a>
Данная проектная работа выполнена в рамках образовательной программы <a href="https://practicum.yandex.ru/">Яндекс Практикума</a>. Проект представляет собой <a href="">продолжение</a> портирования на "React" адаптивного приложения (SPA) с профилем пользователя и фотокарточками, <a href="https://github.com/are-new-ta/mesto">изначально написанного</a> на нативных технологиях: HTML5, CSS3 и JavaScript. В сравнении с предыдущей работой в данном проекте добавлен функционал регистрации и авторизации пользователей на сайте в своем личном кабинете, а также исправлены некоторые ошибки, пропущенные ревьюером

<h4>Ссылка на макеты:
<br>
https://www.figma.com/file/2cn9N9jSkmxD84oJik7xL7/JavaScript.-Sprint-4?node-id=0%3A1
https://www.figma.com/file/bjyvbKKJN2naO0ucURl2Z0/JavaScript.-Sprint-5?node-id=0%3A1
https://www.figma.com/file/kRVLKwYG3d1HGLvh7JFWRT/JavaScript.-Sprint-6?node-id=0%3A1
https://www.figma.com/file/PSdQFRHoxXJFs2FH8IXViF/JavaScript-9-sprint?node-id=0%3A1
https://www.figma.com/file/5H3gsn5lIGPwzBPby9jAOo/Sprint-14-RU?node-id=0%3A1
<br>
</h4>

<i>* - проект прошел код-ревью</i>

<div align="right">(<a href="#summary">к оглавлению</a>)</div>

<a name="technologies"><h2>2. Стек технологий</h2></a>
<span>
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="Иконка React">
  <img src="https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white" alt="Иконка React Router">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="Иконка CSS3">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="Иконка HTML5">
</span>

<div align="right">(<a href="#summary">к оглавлению</a>)</div>

<a name="installation"><h2>3. Установка и запуск приложения в локальном репозитории, эксплуатация (пп. 4-5 актуальны также при работе на Github Pages)</h2></a>
1. `git clone https://github.com/are-new-ta/react-mesto-auth.git` - клонировать репозиторий (с использованием HTTPS) на свое устройство
2. `npm i` - установить зависимости
3. `npm run start` - запустить приложение в режиме разработчика (в браузере ввести ссылку `http://localhost:3000/react-mesto-auth/sign-in`, если приложение не открылось там автоматически)
4. При использовании приложения для входа в личный кабинет пользователю требуется <b>зарегистрироваться</b> и пройти <b>авторизацию</b>.
5. При авторизации в локальном хранилище сохраняется токен пользователя, который при закрытии вкладки с приложением и возвращении позволяет оставаться авторизованным на сайте. Он удаляется после нажатия на кнопку выхода из личного кабинета
<a name="problem-routes">
  <p>
    <b>NB!</b> В связи <a href="https://create-react-app.dev/docs/deployment/#notes-on-client-side-routing">с особенностями совместимости</a> Github Pages с модулем маршрутизации (React Router DOM) в удаленном репозитории <b>не рекомендуется</b> обновление страниц приложения, имеющих добавочные эндпоинты к корневой ссылке <b>/react-mesto-auth</b>
  </p>
</a>
<p>
  <b>NB!!</b> На данном этапе не настроена отрисовка ошибок при попытке регистрации пользователя с ранее зарегистрированным электронным адресом, неправильном вводе электронного адреса и/или пароля и т.п. Эти ошибки можно проверить самостоятельно в <b>консоли разработчика</b> во вкладке <b>&laquo;Network&raquo;</b> (ответ с сервера будет выделен красным цветом)
</p>

<div align="right">(<a href="#summary">к оглавлению</a>)</div>

<a name="establishing"><h2>4. Процесс создания</h2></a>
Работа выполнена в <b>1 этап</b>:
<br>
Верстка дополнительных компонентов (стартовых окон с формами регистрации и авторизации пользователей) и элементов (гамбургер-меню, кнопка выхода из личного кабинета), написание функционала

<div align="right">(<a href="#summary">к оглавлению</a>)</div>

<a name="functionality"><h2>5. Функционал</h2></a>
<details>
  <summary>Адаптивный интерфейс <b><i>(в т. ч. новых компонентов и элементов)</i></b></summary>
    <img width="500" src="https://user-images.githubusercontent.com/108838349/216848219-0d443e1e-a711-4803-a78c-6c998a1786f9.gif" alt="Гиф с демонстрацией адаптивного интерфейса приложения">
 </details>

<details>
  <summary>Регистрация и авторизация пользователей</summary>
    <img width="500" src="https://user-images.githubusercontent.com/108838349/216912837-de6a7d00-24fb-49b9-8e65-7982180eb2c5.gif" alt="Гиф с демонстрацией регистрации и авторизации пользователей">
 </details>

<details>
  <summary>Редактирование данных пользователя</summary>
    <img width="500" src="https://user-images.githubusercontent.com/108838349/216848508-481840e7-176a-466e-9a5f-f73f71c051e2.gif" alt="Гиф с демонстрацией редактирования данных пользователя в личном кабинете">
  </details>

<details>
  <summary>Обновление аватара</summary>
    <img width="500" src="https://user-images.githubusercontent.com/108838349/216848611-c9f96a5e-e87f-4755-8fe9-50592c0a62b1.gif" alt="Гиф с демонстрацией обновления аватара пользователя">
</details>

<details>
  <summary>Добавление новой карточки</summary>
     <img width="500" src="https://user-images.githubusercontent.com/108838349/216848713-6efd8c14-089b-476f-b6f4-cbaa213beba3.gif" alt="Гиф с демонстрацией добавления новой карточки">
</details>

<details>
  <summary>Добавление и снятие лайка (включая счетчик лайков)</summary>
    <img width="500" src="https://user-images.githubusercontent.com/108838349/216848788-786b5957-8e4b-4a1e-9b9a-be82d7475c73.gif" alt="Гиф с демонстрацией добавления и снятия лайка (включая счетчик лайков)">
</details>

<details>
  <summary>Удаление карточки <b><i>с модальным окном подтверждения действия</i></b></summary>
     <img width="500" src="https://user-images.githubusercontent.com/108838349/216848877-b47233a0-0bde-4311-a266-326809dc6941.gif" alt="Гиф с демонстрацией удаления карточки">
</details>

<details>
  <summary>Модальное окно успешной/неудачной регистрации на сайте</summary>
    <img width="500" src="https://user-images.githubusercontent.com/108838349/216910166-40745d73-2086-45ec-a348-306336499426.gif" alt="Гиф с демонстрацией модального окна успешной/неудачной регистрации на сайте">
  </details>

<details>
  <summary>Модальное окно с увеличенной фотографией карточки</summary>
     <img width="500" src="https://user-images.githubusercontent.com/108838349/216910652-a8a9272c-1e87-49e0-b983-93c3952b88e8.gif" alt="Гиф с демонстрацией модального окна с увеличенной фотографией карточки">
</details>

<details>
  <summary>Открытие и закрытие модальных окон (по кнопке, <b><i>оверлею</i></b> и <b><i>клавише "Escape"</i></b>)</summary>
     <img width="500" src="https://user-images.githubusercontent.com/108838349/216910652-a8a9272c-1e87-49e0-b983-93c3952b88e8.gif" alt="Гиф с демонстрацией открытия и закрытия модального окна">
  </details>

<details>
  <summary><b><i>Спиннеры загрузки</i></b></summary>
      <img width="500" src="https://user-images.githubusercontent.com/108838349/216848611-c9f96a5e-e87f-4755-8fe9-50592c0a62b1.gif" alt="Гиф с демонстрацией спиннера загрузки на примере модального окна с обновлением аватара">
 </details>

<details>
  <summary><b><i>Валидация форм</i></b></summary>
    <img width="500" src="https://user-images.githubusercontent.com/108838349/216848611-c9f96a5e-e87f-4755-8fe9-50592c0a62b1.gif" alt="Гиф с демонстрацией валидации формы на примере модального окна с обновлением аватара">
</details>

<details>
  <summary><b><i><b><i>Окно предварительной загрузки страницы</i></b></i></b></summary>
    <img width="500" src="https://user-images.githubusercontent.com/108838349/216913189-b1a3c13c-1f28-4291-856e-a43fa92ce29f.gif" alt="Гиф с демонстрацией окна предварительной загрузки страницы">
 </details>

<details><summary><b><i>Страница 404</i></b> (<a href="#problem-routes"><b>не будет видна</b></a> на  Github Pages)</summary>
     <img width="500" src="https://user-images.githubusercontent.com/108838349/215304244-bd854ae2-0066-416d-a516-3b29f4028363.gif">
 </details>

<br>
