# Codeforcescpp-363A
#include <bits/stdc++.h>
using namespace std;

void number(int num) {
	if (num >= 5)
		cout << "-O|" << string(num % 5, 'O') << "-"
			 << string(4 - (num % 5), 'O');
	else
		cout << "O-|" << string(num % 5, 'O') << "-"
			 << string(4 - (num % 5), 'O');
}
int main() {
	int n;
	cin >> n;
	do {
		number(n % 10);
		cout << endl;
		n /= 10;
	} while (n != 0);
  return 0;
}
