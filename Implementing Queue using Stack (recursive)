#include <bits/stdc++.h>
using namespace std;

class Queue {
    public:
	stack<int> s;

	void enQueue(int x)
	{
		s.push(x);
	}

	int pop()
	{
		if (s.empty()) {
			cout << "Q is empty";
			return -1;
		}

		int x = s.top();
		s.pop();

		if (s.empty())
			{return x;}

		int item = pop();
		s.push(x);

		return item;
	}
};

int main()
{
	Queue q;
	q.enQueue(1);
	q.enQueue(2);
	q.enQueue(3);

	cout << q.pop() << '\n';
	cout << q.pop() << '\n';
	cout << q.pop() << '\n';

	return 0;
}
