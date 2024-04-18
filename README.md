# RK-1

Изотова Нина ИУ8-23

Репозиторий для рк-1 вариант 12: https://github.com/joaofaro/KCFcpp

1. Нзавание проекта
```
    KCFcpp
```
2. Краткое описание проекта (одной фразой). (Это скорее для вас может быть полезно, потому что некоторые из проектов интересны сами по себе - коснетесь в современных разработок)
```
    Этот пакет включает в себя класс C++ с несколькими методами отслеживания, основанными на фильтре корреляции в ядре (KCF).
Он также включает исполняемый файл для взаимодействия с тестом VOT benchmark.
```
3. Количество файлов
```bash
$ git ls-files | wc -l
```
```
    14
```
4. Объем всех файлов
```bash
$ git ls-files | xargs wc -c | awk '{total += $1} END {print total}'
```
```
    136610
```
5. Объем исходного кода: cpp, c, h, hpp, cxx, py, pl, php, java, cs, rb, rs, hs
```bash
$ git ls-files | grep -E ".(cpp|c|h|hpp|cxx|py|pl|php|java|cs|rb|rs|hs)$" | xargs wc -c | awk '{total += $1} END {print total}'
```
```
    128128
```
6. Найти, если есть файл .clang-format
```bash
$  find . -name ".clang-format" | wc -l
```
```
0
```

7. Если есть каталог src, то общее количество файлов в каталоге src
```bash
$ find src -type f | wc -l
```
```
    9
```
8. Выписать количество файлов, содержащих слово socket независимо от написания строчными или прописными буквами во всех файлах репозитория.
```bash
$ git grep -l -i "socket" | wc -l
```
```
    0
```
9. Выписать количество файлов, содержащих слово select независимо от написания строчными или прописными буквами во всех файлах репозитория.
```bash
$ git grep -l -i "select" | wc -l
```
```
    2
```
10. Выписать количество раз, сколько, содержится слово Microsoft, Google или Intel независимо от написания строчными или прописными буквами во всех файлах репозитория.
```bash
$ git grep -i -e "Microsoft" -e "Google" -e "Intel" | wc -l
```
```
    2
```
11. Найти расположение файла LICENSE относительно начала репозитория.
```bash
$ find . -name LICENSE*
```
```
./LICENSE
```
12. Вывести строку для файла LICENSE (если он есть), содержащую следующие подпоследовательности символов: BSD, GNU, MIT, APSL, Apache, GPL, AGPL, LGPL
```bash
$ grep -e "BSD" -e "GNU" -e "MIT" -e "APSL" -e "Apache" -e "GPL" -e "AGPL" -e "LGPL" ./LICENSE
```
```
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
```
