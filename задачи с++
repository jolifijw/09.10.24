#include <iostream>
#include <iomanip>

using namespace std;

int main() {
    setlocale(LC_ALL, "ru");
   //1
    
    //int number;

    //cout << "Введите число больше нуля: ";
    //cin >> number;

    //if (number <= 0) {
    //    cout << "Ошибка: Число должно быть больше нуля." << endl;
    //}
 
    //for (int i = 0; number > 0; i++) {
    //    int digit = number % 10; // Получение последней цифры
    //    cout << digit;
    //    number /= 10; // Удаление последней цифры из числа
    //}
    //cout << endl;
    
    //2

    //int number, digit, sum = 0;
    //cout << "Введите число: ";
    //cin >> number;
    //// Переводим число в положительное, если оно отрицательное
    //if (number < 0) {
    //    number = -number;
    //}
    //// Цикл по каждой цифре числа
    //for (int i = 0; number > 0; number /= 10) {
    //    digit = number % 10;  // Получаем последнюю цифру
    //    sum += digit;         // Суммируем цифру
    //}
    //cout << "Сумма цифр числа: " << sum << endl;

    //3


    //int N;
    //cout << "Введите количество дней: ";
    //cin >> N;
    //int totalDistance = 0;
    //for (int i = 1; i <= N; i++) {
    //    // Расстояние в i-й день
    //    int distance = 15 + (i - 1) * 2;
    //    // Добавление расстояния к общему
    //    totalDistance += distance;
    //    }
    //cout << "Общее расстояние: " << totalDistance << " см" << endl;

       //4
    
    //int a = 0;
    //int b = 0;

    //cout << "Введите результат подбрасывания монеты (1 - орел, 2 - решка):" << endl;

    //for (int i = 0; i < 9; i++) {
    //    int c;
    //    cin >> c;
    //    if (c == 1) {
    //        a++;
    //    }
    //    else if (c == 2) {
    //        b++;
    //    }
    //    else {
    //        cout << "Некорректный ввод. Введите 1 или 0." << endl;
    //        i--; // Повторить текущий бросок
    //    }
    //}
    //if (a % 2 == 0) {
    //    cout << "Решение: Положительное" << endl;
    //}
    //else {
    //    cout << "Решение: Отрицательное" << endl;
    //}

    //5-6

    int month, year, startDay;
    cout << "Введите номер месяца (1-12): ";
    cin >> month;
    cout << "Введите год: ";
    cin >> year;
    cout << "Введите номер дня недели для начала месяца (1-7, 1 - понедельник): ";
    cin >> startDay;
    // Проверка корректности ввода
    if (month < 1 || month > 12 || startDay < 1 || startDay > 7) {
        cout << "Некорректный ввод. Программа завершена." << endl;
        return 1;
    }
    // Определение количества дней в месяце
    int daysInMonth[] = { 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31 };
    if ((year % 4 == 0 && year % 100 != 0) || year % 400 == 0) {
        daysInMonth[1] = 29; // високосный год
    }
    // Вывод заголовка
    cout << "\nКалендарь на " << month << " месяц " << year << " года:\n" << endl;
    cout << "Пн Вт Ср Чт Пт Сб Вс" << endl;
    // Вывод пустых клеток до начала месяца
    for (int i = 1; i < startDay; ++i) {
        cout << setw(3) << " ";
    }
    // Вывод календаря
    int day = 1;
    for (int i = startDay; i <= daysInMonth[month - 1] + startDay - 1; ++i) {
        cout << setw(3) << day++;

        if (i % 7 == 0) {
            cout << endl;
        }
    }
    // Бонусное задание: определение количества выходных
    int weekends = 0;
    for (int i = startDay; i <= daysInMonth[month - 1] + startDay - 1; ++i) {
        if (i % 7 == 6 || i % 7 == 0) { // Суббота или воскресенье
            weekends++;
        }
    }
    cout << "\nВ этом месяце " << weekends << " выходных дней." << endl;

    return 0;
}
