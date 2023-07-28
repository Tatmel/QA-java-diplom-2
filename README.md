<h1 align="center">Второе задание дипломного проекта</h1>
<h2 align ="center" style = "margin-top: -20px">Тестирование API для Stellar Burgers</h2>

  <p align="center" id="project-name">
    Яндекс.Практикум: Дипломная работа, Задание 2
    <br />
    <a href="https://github.com/Tatmel/QA-java-displom-2"><strong>git *</strong></a>
    <a href="https://code.s3.yandex.net/qa-automation-engineer/java/cheatsheets/paid-track/diplom/api-documentation.pdf"><strong>docs API *</strong></a>
    <a href="https://stellarburgers.nomoreparties.site/"><strong>site</strong></a>
    <br />

  </p>



<!-- Содержание -->
<details>
  <summary><b>Содержание</b></summary>
  <ol>
    <li><a href="#tasks">Задачи проекта</a></li>
    <li><a href="#technologies">Использованные технологии</a></li>
    <li><a href="#start-tests">Генерирование отчета</a></li>
  </ol>
</details>



<!-- Задачи проекта -->
<h2 id="tasks">Задачи проекта</h2>

_**Общее описание:**_
<p>Тестирование API для Stellar Burgers.</p>

_**Протестировать ручки:**_
1. Создание пользователя:
<p style="margin: 5px 30px;">a) создание уникального пользователя;</p>
<p style="margin: 5px 30px;">б) создание пользователя, который уже зарегистрирован;</p>
<p style="margin: 5px 30px;">в) создание пользователя без заполненного обязательного поля.</p>

2. Логин пользователя:
<p style="margin: 5px 30px;">a) логин под существующим пользователем;</p>
<p style="margin: 5px 30px;">б) логин с неверным логином и паролем.</p>


3. Изменение данных пользователя:
<p style="margin: 5px 30px;">a) изменение данных пользователя с авторизацией;</p>
<p style="margin: 5px 30px;">б) изменение данных пользователя без авторизации.</p>

4. Создание заказа:
<p style="margin: 5px 30px;">a) создание заказа с авторизацией;</p>
<p style="margin: 5px 30px;">б) создание заказа без авторизации;</p>
<p style="margin: 5px 30px;">в) создание заказа с ингредиентами;</p>
<p style="margin: 5px 30px;">г) создание заказа без ингредиентов;</p>
<p style="margin: 5px 30px;">д) создание заказа с неверным хешем ингредиентов.</p>

5. Получение заказов конкретного пользователя:
<p style="margin: 5px 30px;">a) получение заказов конкретного пользователя, когда тот авторизован;</p>
<p style="margin: 5px 30px;">б) получение заказов конкретного пользователя без авторизации.</p>

<!-- Использованные технологии -->
<h2 id="technologies">Использованные технологии</h2>

В проекте были использованы следующие фреймворки/библиотеки:
* Java 11,
* JUnit 4.13.2,
* RestAssured 5.3.0,
* Allure-junit4 2.22.0,
* GSON 2.10.1

<p align="right">(<a href="#project-name">back to top</a>)</p>



<!-- Генерирование отчета -->
<h2 id="start-tests">Генерирование отчета</h2>

* mvn
  ```sh
  mvn clean test
  ```
* mvn
  ```sh
  mvn allure:serve
  ```

<p align="right">(<a href="#project-name">back to top</a>)</p>