# Lecture 12 Arrays

//EXERCISES

  
Months of the Year

    #include <iostream>
    #include <string>
    using namespace std;
    int main()
    {
        string months[12] = { "January", "February", "March","April","May","June","July","August","September","October","November","December" };

        for (int i = 0; i < 12; i++)
        {
            cout << months[i] << endl;
        }
    }

  

Time Travel
                                 
    #include <iostream>
    using namespace std;
    int main()
    {
      string months[12] = {"January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December" };
      for (int i = 0; i < 12; i++) {
        out << months[i] << endl; }
    }

                     
                            
Marks

        #include <iostream>
        #include <array>
        #include <string>
        #include <algorithm>
        using namespace std;

        int main()
        {
            cout << "\nEnter your score for five subjects";
            int marks[5];
            int sum = 0;
            for (int i = 0; i < 5; i++)
            {
                cout << "\nInput the subject marks" << endl;
                cin >> marks[i];
                while (cin.fail() || marks[i] > 100 || marks[i] < 0) {
                    cout << "invalid command, enter the marks again\n";
                    cin.clear();
                    cin.ignore();
                    cin >> marks[i];
                }

                sum = sum + marks[i];
            }
            cout << "\nYour average is: " << sum / 5 << endl;
        }

Version (1)

    #include <iostream>
    using namespace std;
    int main()
    {
      int marks[5];
      int sum = 0;

      cout << "Enter 5 of your Subejct Marks: " << endl;

      for (int m = 0; m < 5; ++m) {
        cin >> marks[m];
      }

      cout << "\nYour Subject marks are: ";

      for (int s = 0; s < 5; ++s) {
        cout << marks[s] << ", ";
        sum += marks[s] ;

      }
      cout << "\n\nTotal marks = " << sum << "\n";
      cout << "\nAverage marks = " << sum/5 << "\n";
    }
    
    

//NOT EXERCISES

Example initialisation (longhand)

    #include <iostream>
    using namespace std;
    int main()
    {
      int ages[5];

      ages[0] = 19;
      ages[1] = 23;
      ages[2] = 22;
      ages[3] = 30;
      ages[4] = 18;
      }
      
      
Example initialisation (shorthand)

      #include <iostream>
    using namespace std;
    int main()
    {
      int array[5] = { 19, 23, 22, 30, 18 };
    }

Months

Version (1)

    #include <iostream>
    using namespace std;
    int main()
    {
      int days[13];
      int arrays[13] = {0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12 };

      string months[13] = { "months", "January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"};
    }


Version (2)

    #include <iostream>
    using namespace std;
    int main()
    {
      string months[12] = { "January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"};
    }

  
  
Accessing array values
  
    #include <iostream>
    using namespace std;
    int main()
    {
      int heartRates[8] = { 54, 60, 71, 59, 62, 63, 60, 58 };

      cout << heartRates[3] << endl;
      cout << heartRates[6] << endl;
    }

  
  
Iterating through an array
  
    #include <iostream>
    using namespace std;
    int main()
    {
      int heartRates[8] = { 54, 60, 71, 59, 62, 63, 60, 58 };

      for (int i = 0; i < 8; i++) {
        cout << heartRates[i] << endl; }
    }

















