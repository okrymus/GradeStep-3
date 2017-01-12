// The program grade step 3
// Switch case labs
// Programmer: Panupong Leenawarat
// Last modify: 10/8/15

#include <iostream>
using namespace std;

int main()
{
	double score;

	//Title
	cout << "\t  Assign course grade according to this grading scheme:\n"
		 << "\t                        Lee. Panupong                  \n"
		 << "\t                    grade is \"double\" and            \n"
		 << "\t     there are no if statements or other variables       " << endl << endl;

	cout << "\n\t (94, 100] :  A"
		 << "\n\t (84,  94] :  B"
		 << "\n\t (74,  84] :  C"
		 << "\n\t (64,  74] :  D"
		 << "\n\t [ 0,  64] :  F\n\n";

	while (true)
	{
		cout << "What is the average grade? ";
		cin >> score;    cin.ignore(80, '\n');

		cout << "The letter grade is \'";
		switch ((int)ceil((score/10.0) - 0.4))
		{
		case  10:	cout << "A";	break;
		case   9:	cout << "B";	break;
		case   8:	cout << "C";	break;
		case   7:	cout << "D";	break;
		default:	cout << "F";
		}
		cout << "\' because your grade was " << score << endl << endl;
	}
	return 0;
}