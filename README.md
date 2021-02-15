# Lab-13.10-
#include <iostream>
using namespace std;

int main() { // 1. yes the program functions properly
 int month = 1;  
   float total = 0, rain; 
   

   cout << "Enter the total rainfall for month " << month << endl;
   cout << "Enter -1 when you are finished" << endl;
   cin >> rain;

   while (rain != -1) // 2. the purpose of the rain variable is what is being used in the loop 
   {
      total = total + rain; // 4. the total varible is for more accuracy 
      month = month + 1;

      cout << "Enter the total rainfall in inches for month "
           << month << endl;
      cout << "Enter -1 when you are finished" << endl;
      cin >> rain;
   }

   if (month == 1)// 3. Purpose of the month variable is what we are testing for 
      cout << "No data has been entered" << endl;
   else
      cout << "The total rainfall for the " << month-1
           << " months is "<< total << " inches." << endl;
}
// 5. if you answer -1 first line 24 will go and nothing will happen 
// 6. if you enter 0 for more than one month it will still go through the loop until you enter -1
// 7. you should not enter anything negative unless it is -1 to end the loop 
