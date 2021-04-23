[Journal 8.docx](https://github.com/typel2009/Cplusplus-Program/files/6367775/Journal.8.docx)

#include <iostream>
#include <vector>
#include <iomanip>

using namespace std;

double apples; 				// declaring variables
double signedKygerRookieCard;
double beets;
double broccoli;
double cantaloupe;
double celery;
double cranberries;
double cucumbers;
double garlic;
double onions;
double peas;
double potatoes;
double pumpkins;
double radishes;
double spinach;
double yams;
double zuccini;
int userInput;

//creating vector pair
vector<pair<string, int>> groceries{ {"Apples",0}, {"SignedKygerRookieCard",0}, {"Beets",0}, {"Broccoli",0}, {"Cantaloupe",0}, {"Celery",0}, {"Cranberries",0}, {"Cucumbers",0}, {"Garlic",0}, {"Onions",0}, {"Peas",0}, {"Potatoes",0}, {"Pumpkins",0}, {"Radishes",0},{"Spinash",0},{"Yams",0},{"Zuccini",0} };

int main()
{
	// display for user input
	cout << "Welcome Valuable Employee to Corner Grocer's Grocery Counter." << endl;
	cout << "1 = Apples" << endl;
	cout << "2 = Kyger Rookie Card" << endl;
	cout << "3 = Beets" << endl;
	cout << "4 = Broccoli" << endl;
	cout << "5 = Cantaloupe" << endl;
	cout << "6 = Celery" << endl;
	cout << "7 = Cranberries" << endl;
	cout << "8 = Cucumbers" << endl;
	cout << "9 = Garlic" << endl;
	cout << "10 = Onions" << endl;
	cout << "11 = Peas" << endl;
	cout << "12 = Potatoes" << endl;
	cout << "13 = Pumpkins" << endl;
	cout << "14 = Radishes" << endl;
	cout << "15 = Spinach" << endl;
	cout << "16 = Yams" << endl;
	cout << "17 = Zuccini" << endl;



	//while loop to display total of grocery item and to validate the user input
	cout << "Type the number that corresponds to the item purchased (type in a character to exit) " << endl;
	while (!cin.fail() && userInput != 'q')
	{
		cin >> userInput;
		cout << "You entered " << userInput << endl;

		if (userInput == 1)
		{
			groceries[0].second++;
			cout << setw(21) << groceries[0].first << "	";
			cout << groceries[0].second << endl;
		}
		if (userInput == 2) {
			groceries[1].second++;
			cout << setw(21) << groceries[1].first << "	";
			cout << groceries[1].second << endl;

		}
		if (userInput == 3) {
			groceries[2].second++;
			cout << setw(21) << groceries[2].first << "	";
			cout << groceries[2].second << endl;

		}
		if (userInput == 4) {
			groceries[3].second++;
			cout << setw(21) << groceries[3].first << "	";
			cout << groceries[3].second << endl;

		}
		if (userInput == 5) {
			groceries[4].second++;
			cout << setw(21) << groceries[4].first << "	";
			cout << groceries[4].second << endl;

		}
		if (userInput == 6) {
			groceries[5].second++;
			cout << setw(21) << groceries[5].first << "	";
			cout << groceries[5].second << endl;

		}
		if (userInput == 7) {
			groceries[6].second++;
			cout << setw(21) << groceries[6].first << "	";
			cout << groceries[6].second << endl;

		}
		if (userInput == 8) {
			groceries[7].second++;
			cout << setw(21) << groceries[7].first << "	";
			cout << groceries[7].second << endl;

		}
		if (userInput == 9) {
			groceries[8].second++;
			cout << setw(21) << groceries[8].first << "	";
			cout << groceries[8].second << endl;

		}
		if (userInput == 10) {
			groceries[9].second++;
			cout << setw(21) << groceries[9].first << "	";
			cout << groceries[9].second << endl;

		}
		if (userInput == 11) {
			groceries[10].second++;
			cout << setw(21) << groceries[10].first << "	";
			cout << groceries[10].second << endl;

		}
		if (userInput == 12) {
			groceries[11].second++;
			cout << setw(21) << groceries[11].first << "	";
			cout << groceries[11].second << endl;
		}
		if (userInput == 13) {
			groceries[12].second++;
			cout << setw(21) << groceries[12].first << "	";
			cout << groceries[12].second << endl;

		}
		if (userInput == 14) {
			groceries[13].second++;
			cout << setw(21) << groceries[13].first << "	";
			cout << groceries[13].second << endl;

		}
		if (userInput == 15) {
			groceries[14].second++;
			cout << setw(21) << groceries[14].first << "	";
			cout << groceries[14].second << endl;
		}
		if (userInput == 16) {
			groceries[15].second++;
			cout << setw(21) << groceries[15].first << "	";
			cout << groceries[15].second << endl;

		}
		if (userInput == 17) {
			groceries[16].second++;
			cout << setw(21) << groceries[16].first << "	";
			cout << groceries[16].second << endl;

		}
		// exit key
		if (userInput == 'q')
		{
			cout << "Thank you for using Corner Grocer's Grocery Counter" << endl;
			break;
		}

		cout << "\nType the number that corresponds to the item purchased (type any character to exit) " << endl;
	}
	//display histogram with item name and number of ‘*’
	cout << "\tGrocery Item Histogram" << endl;
	cout << "\t----------------------" << endl;
	int i;
	for (auto x : groceries)
	{
		cout << setw(21) << x.first << "	";
		for (int i = 0; i < x.second; i++)
		{
			cout << "*";
		}
		cout << endl;
	}
	return 0;
}
