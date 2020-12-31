#include<iostream>
#include<conio.h>
using namespace std;
int main() {
	int data[10],tp=0;
	cout << "Enter 10 numbers " << endl;
	for (int i = 0; i < 10; i++)
	{
		cin>>data[i];
}
	for (int i = 0; i < 9; i++) {
		for (int j = 0; j < 9 - i; j++) {
			if (data[j] < data[j + 1]) {
				tp = data[j];
				data[j] = data[j + 1];
				data[j + 1] = tp;
			}

			
		}
	}
	cout << "  List in desending order" << endl;
	for (int q = 0; q < 10; q++) {
		cout <<" "<< data[q] << endl;

	}





	_getch();

}
