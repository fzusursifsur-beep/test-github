# Cat and Mouse Game

Консольный проект на C# (.NET 8), переработанный с разделением ответственности между классами.

## Структура

- `CatAndMouseGame/Program.cs` — запуск программы и выбор номера теста.
- `CatAndMouseGame/Player.cs` — игрок, состояние, позиция и перемещение.
- `CatAndMouseGame/Game.cs` — игровая логика и проверка поимки.
- `CatAndMouseGame/GameFileProcessor.cs` — чтение команд и запись отчёта.
- `CatAndMouseGame/CatAndMouseGame.csproj` — настройки проекта.

## Запуск

Откройте `CatAndMouseGame/CatAndMouseGame.csproj` в Visual Studio или выполните из каталога проекта:

```bash
dotnet run
```

Программа просит выбрать тест с номером от 1 до 4. Для работы соответствующий файл данных (`1.ChaseData.txt`, `2.ChaseData.txt`, `3.ChaseData.txt` или `4.ChaseData.txt`) должен находиться в рабочем каталоге приложения. Первая строка файла содержит размер поля; далее идут команды игроков (`C` — кот, `M` — мышь) и `P` для записи текущих позиций в отчёт.

Результат сохраняется в файл `N.PursuitLog.txt`, где `N` — номер выбранного теста.
