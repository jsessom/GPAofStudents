# GPAofStudents
Finding the average grade for however many students you may have.
#include <iostream>
#include <math.h>
#include <iomanip>
#include <string>

using namespace std;
int main()
{
	double GPA,  product,  sum, courseaverage;
	int exam1, exam2, exam3,course, LCV, size, numofcourse;

	cout << " Please enter the number of students you wish to input data. \n";
	cin >> size;



		for (LCV = 0; LCV < size; LCV++)

		{
			cout << " Please enter the amount of courses the student is taking. ";
			 cin>>numofcourse;

			int loop;
			for (LCV = 0; LCV < numofcourse; LCV++)
			{


				cout << " Please enter the grade for exam one. \n";
				cin >> exam1;

				cout << " Please enter the grade for exam two. \n";
				cin >> exam2;

				cout << " Please enter the grade for exam three. \n";
				cin >> exam3;

				courseaverage = (exam1 + exam2 + exam3) / 3;
				cout << " The average grade for the course is " << courseaverage << "." << endl;
				cout << endl;


				if (courseaverage >= 90 && courseaverage <= 100)
				{
					GPA = 4.0;
					cout << " The GPA of the student is " << GPA << "." << endl;
					cout << endl;
				}

				else if (courseaverage >= 80 && courseaverage <= 89)
				{
					GPA = 3.0;
					cout << " The GPA of the student is " << GPA << "." << endl;
					cout << endl;
				}

				else if (courseaverage >= 70 && courseaverage <= 79)
				{
					GPA = 2.5;
					cout << " The GPA of the student is " << GPA << "." << endl;
					cout << endl;
				}

				else if (courseaverage >= 60 && courseaverage <= 69)
				{
					GPA = 2.0;
					cout << " The GPA of the student is " << GPA << "." << endl;
					cout << endl;

				}

				else
				{
					GPA = 1.0;
					cout << " The GPA of the student is " << GPA << "." << endl;
					cout << endl;
				}
			}
		}

	system("pause");
	return 0;

