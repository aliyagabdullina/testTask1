# Тестовое задание Габдуллина Алия
Программа на Python для обработки файлов.

Программа принимает входные параметры тремя способами: 

    1. Напрямую, при вызове функции из кода Python.
    
    2. Через параметры командной строки.
    
    3. Через переменные окружения.
    
Функция copy_files_with_english_chars копирует файлы, содержащие английские символы, в указанную целевую директорию. 

Функция принимает на вход список файлов и целевую директорию, которая может быть None, если директория задается после вызова функции. 

Функция содержит в себе проверку на корректность введенных данных и непосредственно проверку на наличие английских символов и копирование файлов в случае выполнения всех условий (В файле должен быть хотя бы один английский символ)

Код также включает набор тестов, которые можно использовать для проверки правильности работы функции copy_files_with_english_chars.

Запустить тесты можно выполнив в терминале команду `pytest test.py`

Описание тестов:

1. test_non_english_chars_direct: Проверяет, что файл с содержимым на русском языке не копируется, и выводится соответствующее сообщение на консоль.

2. test_english_chars_direct: Проверяет, что файл с содержимым на английском языке успешно копируется.

3. test_mixed_chars: Проверяет, что файл с смешанным содержимым (английские и русские символы) успешно копируется.

4. test_multiple_files: Проверяет, что только файлы с содержимым на английском языке копируются, а файлы с неанглийским содержимым не копируются. Проверяет вывод в консоль.

5. test_copy_files_with_nonexistent_file: Обрабатывает ситуацию, когда указанный файл не существует. Проверяет, что выводится сообщение о несуществующем файле.

6. test_directory_as_file: Обрабатывает ситуацию, когда указанный путь является директорией вместо файла. Проверяет, что выводится сообщение о некорректном пути.

7. test_invalid_target_directory: Обрабатывает ситуацию, когда указанная целевая директория не существует или не является директорией. Проверяет, что выводится сообщение о некорректной директории.

8. test_from_command_line: Проверяет корректность передачи пути к файлу через командную строку. 

9. test_from_environment: Проверяет корректность передачи пути к файлу через переменную окружения. 


Запустив тесты, получим следующий результат: 


![Фото](images/tests.png)
