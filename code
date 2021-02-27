//
//  main.cpp
//  Project 2
//
//  Created by Max Matkovski on 1/18/21.
//

#include <iostream>
using namespace std;

int main() {
    
// Declaring Variables
    string Month;
    int Day = 0;
    int Year = 0;
    int MonthCode = 0;
    int LeapYear = 0;
    int LeapYearMonth = 0;
    int LeapYearPassed = 0;
    int CenturyValue = 0;
    int CenturyCode = 0;
    int YearCode = 0;
    int DayCode = 0;
    string DayOfWeek;
    
// Prompt for Month
   cout << "Provide a month:\n";
    cin >> Month;
    
    
// Validating for Month Input
    if (Month == "January" or Month == "February" or Month == "March" or Month == "April" or Month == "May" or Month == "June" or Month == "July" or Month == "August" or Month == "September" or Month == "October" or Month == "November" or Month == "December"){
    }
        
// Print Error Month Message
    else {
        cout << "Invalid month!\n";}
    
// Assign MonthCode based off of Month
    if (Month == "January"){
        MonthCode = 1;
    }
    
    if (Month == "February"){
        MonthCode = 4;
    }
    
    if (Month == "March"){
        MonthCode = 4;
    }
    
    if (Month == "April"){
        MonthCode = 0;
    }

    if (Month == "May"){
        MonthCode = 2;
    }
    
    if (Month == "June"){
        MonthCode = 5;
        
    } if (Month == "July"){
        MonthCode = 0;
    }
    
    if (Month == "August"){
        MonthCode = 3;
    }
    
    if (Month == "September"){
        MonthCode = 6;
    }
    
    if (Month == "October"){
        MonthCode = 1;
    }
    
    if (Month == "November"){
        MonthCode = 4;
    }
    
    if (Month == "Decemeber"){
        MonthCode = 6;
    }
    
    
// Prompt for Day
    cout << "Provide a day:\n";
     cin >> Day;
    
// Validating Day
    if (1 <= Day and Day <= 31){
    }
    
// Print Error Day Message (if applicable)
    else{
        cout <<"Invalid day!\n";}
    
// Prompt for Year
    cout << "Provide a year:\n";
     cin >> Year;
    
    
// Validating Year
    if (1 <= Year and Year <= 3000){
    }
    else{
        cout <<"Invalid year!\n";}
    

        
// Leap Year (Year Logical Test)
    
    if (Year % 4 == 0){LeapYear = 1;}
    
    if (Year % 100 == 0){LeapYear = 0;}
    
    if (Year % 400 == 0){LeapYear = 1;}
    

// Leap Year (Month Logical Test)
    if (Month == "January" or Month == "February"){LeapYearMonth = 1;}
    
// MonthCode Adjustment if Inputted Year is a Leap Year
    if (LeapYear and LeapYearMonth){LeapYearPassed = 1;}
    
    if (LeapYearPassed){MonthCode = MonthCode - 1;}
    
// CenturyValue Calculation and Value Assignment to CenturyCode
    
   CenturyValue = (Year / 100) % 4;
    
    if (CenturyValue == 0){CenturyCode = -2;}
    if (CenturyValue == 1){CenturyCode = 3;}
    if (CenturyValue == 2){CenturyCode = 1;}
    if (CenturyValue == 3){CenturyCode = -1;}

// YearCode Calculation
    
    YearCode = ((Year % 100) / 4) + (Year % 100);
    
// DayCode Calculation and String Input
    DayCode = (CenturyCode + Day + YearCode + MonthCode) % 7;
    
    
    if (DayCode == 0){DayOfWeek = "Sunday";}
    if (DayCode == 1 or DayCode == - 6){DayOfWeek = "Monday";}
    if (DayCode == 2 or DayCode == - 5){DayOfWeek = "Tuesday";}
    if (DayCode == 3 or DayCode == - 4){DayOfWeek = "Wednesday";}
    if (DayCode == 4 or DayCode == - 3){DayOfWeek = "Thursday";}
    if (DayCode == 5 or DayCode == - 2){DayOfWeek = "Friday";}
    if (DayCode == 6 or DayCode == - 1){DayOfWeek = "Saturday";}
  
// Final Message
    cout << Month << " " << Day << ", " << Year << " was a " << DayOfWeek << "!\n";
    
// End of Program
    return 0;
    
}
