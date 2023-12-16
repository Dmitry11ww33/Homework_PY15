# Homework_PY15
Ex.1

Дан текстовый файл. Написать функцию, которая составляет шифр для цифр (шифр можете придумать свой, вот пример 1 → ! | 2 → @  | 3 → #  |  4 → $  и т.д.), возвращаемое значение должно быть типа string.
Применить эту функция для файла и заменить все цифры на зашифрованные значения


def find_txt_files(filename):
    result = []
    with open(filename, 'r') as file:
        content = file.read()
        files = content.split()
        for file in files:
            if '.txt' in file:
                result.append(file.replace(' ', ''))
    return result
file_list = find_txt_files('текстовый_файл.txt')
print(file_list)
