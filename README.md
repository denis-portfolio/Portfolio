# Портфолио: инженер по тестированию

## Обо мне 

Привет! Меня зовут ``Денис``, я начинающий тестировщик. <br>
В этом репозитории вы можете найти некоторые из моих проектов, выполненных во время обучения и практики.
<br>

## Навыки и технологии
``Jira``,``qase.io``,``SQL``,`` Postman``, ``Swagger``, ``Trello``, <br>
``SoapUI``, ``Git``, ``Chrome DevTools``, ``Miro``, ``pgAdmin``, ``Mockoon``, ``Confluence``.




## Проекты
### Проект 1: тест веб-приложения для учителей от Skyeng
<p>Продукт: Веб-приложение для учителей от Skyeng, вкладка «Расписание»</P>
<P>Заказчик: учителя онлайн-школы "Skyeng"</P>
<P>Основные требования (главная user-story): предоставить возможность учителям использовать личные события в расписании, которые служат напоминанием, что что-то запланировано на это время.</P>

<p>Что нужно было сделать:</p>
<ol>
  <li>Для тестирования веб-приложения для учителей Skyeng были составлены и проведены следующие виды тестирования:
<ul>
  <li>Приемочные тест-кейсы по требованиям стейкхолдеров;</li>
<li>Тестирование требований проводилось для того, чтобы требования были понятны и однозначны для всех, полными и не противоречивыми;</li>
<li>Smoke-тестирование. Проверка критически важных функций и стабильности системы в целом перед более тщательное тестированием.;</li>
<li>Функциональное тестирование - чек-лист;</li>
<li>Регрессивное тестирование итогового проекта.</li>
  </ul>
  </li>
  <li>Была создана декомпозиция веб-приложения для учителей от Skyeng, вкладка "Расписание";</li>
  <li>Составлено расписание тестирования: кто из тестировщиков и когда будет проводить своё тестирование (в данном проекте тестировщик был один - я, поэтому составил таблицу с этапами проекта и когда с ними работал);</li>
  <li>Во время проведения тестирования были обнаружены баги во вкладке "Расписание" как в новом функционале «Личные собития», так и в старом "Урок";</li>
  <li>В завершении проекта был составлен отчёт о проведённом тестировании, где указаны виды тестирования, сколько было затрачено время на проект, описаны баги и результаты по проекту.</li>
</ol>
<p>В данном проекте были использованы такие инструменты: <strong>"qase.io", "checkVist", "Confluence", "Jira", "Miro"</strong></p>
<p>Как решал:</p>
> <a href=https://>Ссылка на проект</a>
 
 <p><strong>Выводы (Итоги):</strong></p>
  <ol>
         <li>Составил тест-план;</li>
         <li>Подготовил тестовую документацию;</li>
         <li>Провел несколько видов тестирования (приёмочное, функциональное, smoke-tetting и регрессивное);</li>
         <li>Написал подробный отчёт о проведённых результатах тестирования.</li>
  </ol>
         
### Проект 2: тест кабинета учителя в приложении Skyeng
#### Проект 2 является продолжением Проекта 1, только тут мы в тестирование добавляем API.

<p><strong>Продукт:</strong> Веб-приложение для учителей от Skyeng, вкладка "Расписание"</p>
<p>Заказчик: учителя онлайн-школы "Skyeng"</p>
<p>Основные требования (главная user-story): предоставить возможность учителям использовать личные события в расписании, которые служат напоминанием, что что-то запланировано на это время.</p>

<p>Что нужно было сделать:</p>
<ol>
  <li>К ранее созданным тест-кейсам Проекта 1 добавил тест-кейсы для API;</li>
  <li>Коллекция для проведения тестирование API содержала:
    <ul>
      <li>Метод POST, так как в документации к проекту был указан только этот метод;</li>
      <li>10 различных проверок как позитивные, так и негативные:</li></ul>
      <ul>
        <li>Основная Бизнес Логика функции "Личные События"</li>
        <li>Личное Событие занести прошедшей датой</li>
        <li>Личное Событие занести датой из будущего</li>
        <li>Проверка поля Название при добавление Личного События в расписание</li>
        <li>Выборать диапазон времени для Личного События</li>
        <li>Проверка поля Описание при добавлении Личного События в расписание</li>
        <li>Проверка функции Цвет события в Личном Событии</li>
        <li>Проверка совмещения двух Личных Событий в одно время</li>
        <li>Проверка функции Редактирования Личного События</li>
        <li>Редактировать несуществующего Личного События</li>
      </ul>
  <li>В "Variables" были занесены такие данные как ссылка на веб-приложение и токен и заменены на свои значения "Url", "nevToken";</li>
  <li>Использовались скрипты для запоминания id, времени создания события:</li>
  var key = "idLS"
var value = pm.response.json().data.payload.id
pm.collectionVariables.set(key, value);

var key = "startAt"
var value = pm.response.json().data.startAt
pm.collectionVariables.set(key, value);
  </li>
  <li>В завершении тестирования Проекта 2 был дополнен отчёт об тест-ране API-коллекции в результатах тестирования Проекта 1.</li>
  </ol>
  
