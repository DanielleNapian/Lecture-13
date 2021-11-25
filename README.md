# Lecture-13
ranged based for loop

    #include <iostream>
    #include <string>
    using namespace std;

    int main()
    {
        string courses[] = { "BSU CC", "BSU BA", "HNC CC", "HND" };

        for (int i = 0; i < 4; i++) {
            cout << courses[i] << endl;
        }
        for (auto course : courses) {

        }
    }


auto keyeword
                                  
    #include <iostream>
    #include <string>
    using namespace std;

    int main()
    {
        char letters[] = { 'C', 'o', 'd', 'e', 'L', 'a', 'b' };
        for (auto letter : letter) {
            cout << letter << end;
        }
    }
                                
input output
    
    #include <iostream>
    #include <string>
    using namespace std;
    int main()
    {
        int courses[5];

        for (int i = 0; i < 5; i++) {
            cout << "Input the " << i + 1 << " number" << endl;
            cin >> courses[i];
            while (cin.fail()) {
                cout << "invalid command, enter the number again\n";
                cin.clear();
                cin.ignore();
                cin >> courses[i];
            }
        }
        cout << "the numbers are: \n";
        for (auto course : courses) {//range based for loop
            cout << course << endl;
        }


    }    
array art
    
    #include <iostream>
    #include <string>
    using namespace std;
    int main()
    {
        string snacks[5][5] = {
            {"_","_","_","_","_"}, //1 row
        {"_", "O", "_", "O", "_"}, //2 row
        {"_", "@", "@", "@", "_"}, //3 row
        {"_", "^", "^", "^", "_"}, //4 row
        {"_", "V", "V", "V","_" } //5 row
        };

        for (int x = 0; x < 5; x++)
        {
            cout << endl;
            for (int y = 0; y < 5; y++)
                cout << snacks[x][y];
        }
        cout << endl;
    }    
2D arrays
    
    #include <iostream>
    #include <string>
    using namespace std;

    int main()
    {
        string snacks[3][4] = {
            {"Galaxy silk", "Mars Bar", "Snickers", "Bounty"},
            {"Flavoured youghurt","Oman chips","Oreo","Lays"},
            {"Apple", "Banana", "Orange", "Pear"}
        };

        for (int i = 0; i < 3; i++) {
            for (int j = 0; j < 4; j++) {
                cout << snacks[i][j] << "";
            }
            cout << endl;
        }
    }
