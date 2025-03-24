# pytest_redfish
Разработка автотестов для API Redfish с использованием PyTest

## Перечисление автотестов
В набор входят следующие тесты:
- Тест аутентификации в OpenBMC через Redfish API
- Тест получения информации о системе
- Тест управления питанием системы (включение/выключение сервера)

## Результат тестирования

1. Для запуска программы, содержащей тестовые функции, необходимо использовать команду:
   ```
   pytest -rf test_redfish.py
   ```

2. После выполнения функций в терминале будет отображен результат прохождения тестов и время их выполнения.

   ![test_redfish_run](https://github.com/Doom-ux/pytest_redfish/blob/media/test_redfish_run2.png)

3. В дальнейшем для сохранения логов тестовых функций в файл необходимо запускать программу следующим образом:
   ```
   pytest -rf test_redfish.py >>test_output.log && echo " " >>test_output.log
   ```

## Структура каталогов

```
pytest_redfish/
    test/
        test_output.log
        test_redfish.py
        __pycache__/
            test_redfish.cpython-312-pytest-8.3.5.pyc
    README.md
```
