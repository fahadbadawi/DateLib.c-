# Date Library (clsDate) 📅

A comprehensive C++ Date Management Library built using Object-Oriented Programming (OOP) principles. This library provides a robust set of tools to handle, validate, and manipulate dates easily.

## ✨ Features
- **System Date Retrieval**: Get the current local system date automatically.
- **Date Validation**: Check if a given date is valid (handles leap years and month lengths).
- **Calendar Generator**: Print formatted month or full-year calendars directly to the console.
- **Time Conversions**: Convert years and months into total hours, minutes, and seconds.
- **Day Info**: Calculate day-of-week order and fetch short names (e.g., Sun, Mon).

## 🚀 Usage Example

```cpp
#include <iostream>
#include "Date.h"
using namespace std;
int main()
{
    clsDate Date1;
    Date1.Print();

    clsDate Date2("31/1/2022");
    Date2.Print();

    clsDate Date3(20, 12, 2022);
    Date3.Print();

    clsDate Date4(250, 2022);
    Date4.Print();

    Date1.IncreaseDateByOneMonth();
    Date1.Print();

    Date3.PrintYearCalendar();
    cout << Date2.IsValid() << endl;
    cout << "My Age InDays: " << clsDate::CalculateMyAgeInDays(clsDate(13, 11, 2005));
    system("pause>0");
    return 0;
};
