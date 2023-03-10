# mystore
## Техническое задание для кандидатов:

1. разработка хттп сервера (задание обязательно к выполнению)

Представьте, что вы получили новый проект интернет-магазина и вам нужно заложить архитектуру для его разработки и поддержки. 
В качестве тестовго задания полностью спроектируйте базу данных, а так же сделайте CRUD одной (любой) сущности. 
HTTP сервер должен быть написан на GoLang, масимально просто, без использования фреймворков.

Техническое Задание:
- разработать HTTP API с базовой авторизацией, 
которое будет позволять выполнять CRUD операции над сущностями. 
Пользователь будет один (администратор, который и будет создавать эти сущности)
- формат ответа: JSON
- описание сущностей и полей (если вы считаете, что какого-то поля не хватает, вы можете смело его добавить):
    - продавец (имя, телефон)
    - товар (название, описание, цена, продавец)
    - покупатель (имя, телефон)
    - заказ (покупатель, несколько товаров)


2. оптимизация функции конкатенации. (задание со звездочкой, можно не делать, если не знаете)

Опмтимизируйте скорость выполнения функции. Кол-во значений во входящем параметре (len(str)) >= 30.
Напишите бенчмарк тест на эту функцию и на её оптимизированную версию.

```
func concat(str []string) string  {
    result := ""
    for _, v := range str {
        result += v
    }
    return result
}
```


Выполненное тестовое задание разместите на гитхабе.
Доступ к проекту предоставьте на аккаунт: https://github.com/Kirill-Shkodkin
