# WsQ13.cpp
Babylonian Method


/*
#WSQ13
Main: Babylonian Method
By: Jorge Cervantes
#TC1017
Referencia: YouTube,. (2015). The Babylonian Method. Retrieved 27 March 2015, from https://www.youtube.com/watch?v=b4kWHjplWgY
---------------------------------------------------------------------
*/

#include <iostream>
#include <math.h>

using namespace std;

double El_babyloni(int x){
	double w, y, z, u;

	w = sqrt(x - 1);
	y = sqrt(x + 1);

	z = ( (w + (x/w)) / 2 ) + ( (y + (x/y)) / 2 );
	u = z / 2;

	return u;
}

int main(){
	int x;
	double u;

	cout << "This program will calculate the squaret root of a nomber usisng Babylonian Method. \n";
	cout << "Numero a calculate" << endl;
	cin >> x;

	u = El_babyloni(x);

	cout << "The squaret root of "<< x << " is approximate to "<< u << endl;

	return 0;
}
