# Программа для занесения данных о проектах, сотрудниках и задачах в БД
## ОБЯЗАТЕЛЬНЫЕ ТРЕБОВАНИЯ
Код выполненного задания должен быть структурирован, легко читаем и содержать необходимые комментарии. Написанная вами программа должна являться законченным
программным продуктом, т.е. должна легко устанавливаться, предусматривать обработку нестандартных ситуаций, быть устойчивой к некорректным действиям пользователей и т.д

## ТРЕБОВАНИЯ К ТЕХНОЛОГИЯМ
1) NET C# (EntityFramework, ASP.NET MVC Core);
2) Необходимо использовать бд для хранения данных;
3) Рекомендовано использовать units test для отладки уровня логики;

## Задание 1
Реализовать программу для занесения данных о проектах в базу данных и дальнейшей работы с этими данными.  
Функциональные требования: 
1) Возможность создавать/просматривать/редактировать/удалять информацию о проектах;
2) Возможность создавать/просматривать/редактировать/удалять информацию о работниках;
3) Возможность добавлять и удалять работников c проекта (один сотрудник может работать одновременно на нескольких проектах, и на одном проекте может работать несколько человек);
4) Для просмотра проектов предусмотреть различные способы фильтрации (по диапазону даты начала, по приоритетам, и т.п.) и сортировки (по основным полям).

Необходимая для хранения информация: 
1) Название проекта;
2) Название компании-заказчика;
3) Название компании-исполнителя;
4) Данные о сотруднике (имя, фамилия, отчество, email);
5) Данные о руководителе проекта;
6) Данные об исполнителях проекта;
7) Даты начала и окончания проекта;
8) Приоритет проекта (целочисленный).

## Задание 2
Добавить сущность «Задача», используя Entity Framework Code First DB Migrations.
Функциональные требования:
1) Возможность создавать/просматривать/редактировать/удалять информацию о задачах;
2) Возможность добавлять и удалять задачи из проекта (один проект может содержать несколько задач);
3) Возможность добавлять и менять работников (исполнителей проекта) на задачи (у задачи может быть только один работник, у одного работника может быть много задач);
4) Для просмотра задач предусмотреть различные способы фильтрации (например, по статусу) и сортировки (по основным полям).

Необходимая для хранения информация:
1) Название задачи;
2) Автор задачи (связь с сущностью «Работник»);
3) Исполнитель задачи (связь с сущностью «Работник»);
4) Статус задачи (перечисление ToDo/InProgress/Done);
5) Комментарий;
6) Приоритет задачи (целочисленный).
