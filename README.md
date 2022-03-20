# javarush_cryptocode
## Автор: Вахутко Андрей
### Кратное описание:
Данная программа написана на языке Java и применяется для шифрования/дешифрования файлов
с использованием шивра Цезаря. Для взлома шифра в программе предусмотрен режим BruteForce
(взлом грубой силой) и режим статического анализа (методом анализа слов и анализ с подсчётом частоты
использования букв в тексе).
### Для запуска программы необходимо создать исполняемый jar файл или открыть проект в IntellijIDEA
Запуск программы с использованием jar файла. Открыть командную строку и выполнить команду:
"java -jar *"путь к файлу"*/cryptocode.jar"
### Далее вас приветствует меню:
1. Description:
2. ENCRYPTION - encryption document
3. DECRYPTION - decryption document
4. CRYPTO_BRUTE_FORCE - crypto analysis by brute force method
5. CRYPTO_STATISTIC_ANALYSIS - crypto analysis by statistic analysis
6. Enter EXIT to close or enter a type(ENCRYPTION\DECRYPTION\CRYPTO_BRUTE_FORCE\CRYPTO_STATISTIC_ANALYSIS):
### Для продолжения необходимо выбрать один из режимов работы программы. Необходимо ввести название режима и нажать клавишу "Enter"
### 1. Режим Шифрования (ENCRYPTION):
1. Указываем путь к исходному файлу и нажимаем "Enter"
2. Указываем ключ кодирования и нажимаем "Enter"
3. ИТОГ: получаем зашифрованный файл в директории исходного файла с окончанием "_resolve"
### 2. Режим Дешифровки (DECRYPTION):
1. Указываем путь к файлу для дешифровки и нажимаем "Enter"
2. Указываем ключ декодирования и нажимаем "Enter"
3. ИТОГ: получаем дешифрованный файл в директории зашифрованного файла с окончанием "_decode"
### 3. Режим Грубой Силы (CRYPTO_BRUTE_FORCE):
1. Указываем путь к файлу для дешифровки и нажимаем "Enter"
2. ИТОГ: получаем дешифрованные файл в директории зашифрованного файла с окончанием "_decode" и
номером ключа для взлома. Далее необходимо вручную просмотреть все файлы для поиска корректно
расшифрованного файла
### 4. Режим взлома методом статистического анализа (CRYPTO_STATISTIC_ANALYSIS):
1. Указываем путь к файлу для дешифровки и нажимаем "Enter"
2. Выбираете метод анализа. Анализ с помощью слов (W) или анализ с помощью букв (L). Необходимо
ввести букву "W" или "L" и нажать клавишу "Enter"
3. Для анализа с помощью букв потребуется ввести количество файлов для анализа частоты использования
букв. Далее по очереди необходимо указать пути к файлам для анализа
4. ИТОГ: в консоль выводится список с именами файлов, которые с наибольшей вероятностью удалось
успешно дешифровать. Далее необходимо просмотреть предложенные файлы вручную или проверить остальные
декодированные файлы в каталоге исходного файла