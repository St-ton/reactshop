//! Макет
//! <https://www.figma.com/file/Rn3s2F8VGncbkpEx2JRKnJ/main-project?node-id=0%3A1&t=wUv2u4Ybwu3voLFa-0>

// todo 1) создать страницы - CategoriesPage - BasketPage - AllProductsPage - NotFoundPage и подключить к роутингу

//todo 2) подключить redux и отобразить просто списком названия категорий на странице CategoriesPage массив с категориями задать как defaultState ["electronics", "jewelery", "men's clothing", "women's clothing"];

//todo 3) создать навигационное меню с пунктами
//todo категории
//todo все товары
//todo корзина
//todo реализовать красный бордер для активной страницы

//todo 4) реализовать страницу с категориями как на макете. добавить компонент CategoryItem

//todo 5) используя асинхронные action загрузить из API массив с категориями и отобразить его <https://fakestoreapi.com/products/categories>

//todo 6) используя асинхронные action загрузить из API массив с товарами и отобразить его необходимо вывести только наименования товаров в отдельных параграфах на странице AllProductsPage <https://fakestoreapi.com/products>


// todo 7-10 Задания от 20.03 сюда же записать

// todo 11) добавить новый page ProductDescriptionPage с URL /product/:id
при переходе по указанному адресу на странице должно отображаться название товара

НЕ ДЕЛАТЬ ДОПОЛНИТЕЛЬНЫХ сетевых запросов

// todo 12) добавить переход на странциу с продуктом при нажатии на карточку с продуктом

// todo 1) создать страницу, которая будет отображать товары определенной категории данная страница отображается при переходе по ссылке /category/:category
// todo добавить ее в роутинг НЕ ДОБАВЛЯТЬ В NAV

//todo добавить компонент BasketCalculation в нем должно отображаться общее кол-во единиц продуктов в корзине

// todo добавить компонент BasketItem и реализовать вывод данных как на макете кнопки пока не выполняют никакого функционала

//todo реализовать обработчики на нажатие кнопок при нажатии на + кол - во растет на 1, при нажатии на - кол-во уменьшается на 1

// todo реализовать процесс добавления продукта в корзину и повесить его на кнопки если такой товар в корзине уже есть у него необходимо увеличить count на 1 если такого товара в корзине нет, то добавить его с count = 1

// todo добавить переход на странциу с продуктом при нажатии на карточку с продуктом

//todo   добавить проверку на загруженность продуктов  если продукты еще не загрузились - вывести отбивку "данные грузятся"

//todo добавить новый page ProductDescriptionPage с URL /product/:id при переходе по указанному адресу на странице должно отображаться названи товара
// НЕ ДЕЛАТЬ ДОПОЛНИТЕЛЬНЫХ сетевых запросов

// todo создать третью страницу ProductsPage и в роутинге использовать ее в случае всех товаров и в случае товаров определенной категории внутри компонента ProductsPage необходимо обрабатывать оба перехода с разных ссылок

//todo добавить фильтрацию товаров и выводить только те, у которых show: true

//todo добавить ветку условия PRODUCTS_SEARCH_FILTER в качестве payload мы передаем строку из поля ввода написать map который меняет продукты по следующей схеме если название продукта начинается на указанную строку то show true в ином случае show  false для реализации этой логики используйте метод startsWith

//todo - создать actionCreator  - вызвать dispatch с этим action creator при вводе строки в поле поиска

//todo сделать поиск не регистрозависимым

//todo добавить type PRODUCTS_RESET_FILTER  он проходится по всем товарам и указывает у них true
//todo вызвать dispatch с соответствующим action creator при загрузке ProductsPage

//todo добавить ветку условия для сортировки PRODUCTS_SORT_FILTER при 1 сортировать 0 -> 9  при 2 сортировать 9 -> 0

// todo создать компонент ProductsFilterBarи добавить в него поле ввода при вводе значения оно должно выводиться в консоль

// todo доработать CategoryItem и обернуть его в Link при нажатии на Link должен быть переход на страницу с продуктами соответствующей категории


//todo 1) создать reducer BasketReducer
//todo 2) подключить его к state
//todo 3) указаь значение по умолчанию
//
//[
//    {id: 1, count: 3},
//    {id: 2, count: 5}
//]
// todo 4) на странцие корзины вывести в параграфах id и count


//todo 1) считать все продукты и оставить только те, у которых категория соответствует указанной в URL
//todo 2) пройтись мапом по получившемуся массиву и вывести карточки продуктов
//todo НЕ ДЕЛАЕМ ДОПОЛНИТЕЛЬНЫХ СЕТЕВЫХ ЗАПРОСОВ