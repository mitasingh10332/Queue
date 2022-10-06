
#include <bits/stdc++.h>
using namespace std;
#define n 20

class Queue 
{
	int *ar;
	int front;
	int back;

	public:

	Queue (){ 
	ar=new int[n];
	front =-1;
	back=-1;

	}

	void push(int x) 
	{
		if (back==n-1)
	{ cout<< "Queue overloaded"; return ;}

	   back++;
	   ar[back]=x;
	   if (front==-1)
	   {front++;}

	}

	void pop()
	{
		if (front==-1 || front>back)
		{ cout<<"no element +nt";}

		front++;
	}

	int peek()
	{
		if (front==-1 || front>back)
		{ cout<<"no element +nt";}	

		return ar[front];	
	}

	bool empty ()
	{
		if (front==-1 || front>back)
		{ return true;}
		return false;
	}


};

int main()
{
	Queue q;
	q.push(8);
	cout<<q.peek()<<endl;
	q.push(5);
	cout<<q.peek()<<endl;
	q.pop();
	cout<<q.peek()<<endl;


	
	return 0;
}
