Работа на задание первого этапа регионального конкурса профессионального мастерства «Лучший разработчик WEB и мультимедийных приложений»
=

[Репозиторий](https://github.com/JanWeek/WebCup2019)  
[Ссылка на ресурс Яндекс.Диск, с которого берутся изображения](https://yadi.sk/d/mRaE6cwof42rkw)

Приложение было разработано с использованием следующих инструментов:
* Vue.js (vuex, vue-router)
* Bootstrap 4
* Axios
* Webpack

Был реализован функционал:
* Авторизация пользователя в приложении при помощи сервиса [Яндекс](https://yandex.ru/promo/login)
* Галерея изображений (с модальным окном для каждого отдельного) с подгрузкой изображений через [API Яндекс.Диска](https://tech.yandex.ru/disk/api/concepts/quickstart-docpage/)
* Постраничная навигация списка изображений
* AJAX загрузка страниц навигации
* Адаптивная верстка под различные разрешения экрана с использованием сетки Bootstrap

К сожалению, во время работы с API Яндекса столкнулся с некоторыми проблемами, которые описал комментариями в коде. Буду благодарен за разъяснение!

Все зависимости приложения прописаны в package.json

Для развертывания приложения необходимо воспользоваться менеджером пакетов NPM:

`npm install`,
затем запустить запустить скрипт
`npm run production`

На сайте реализована авторизация через Яндекс OAuth. Для авторизации необходимо нажать на иконку Яндекса в правом верхнем углу в шапке сайта, после чего произойдёт переход на страницу Яндекса, где необходимо подтвердить доступ приложения к данным пользователям.  
После этого появится возможность нажать на иконку с аватаром пользователя из Яндекс.Паспорт и просмотреть данные пользователя.  
Для просмотра увеличенной картинки в галерее необходимо нажать на уменьшеное изображение, и откроется модальное окно просмотра. В нём можно листать изображения на данной странице навигации.  
Изображение можно скачать в полном размере, нажав на кнопку "Скачать файл".
