#include <bits/stdc++.h>
using namespace std;

void printKMax(int arr[], int N, int K)
{

	deque<int> Qi(K);
	vector<int>ans;

	int i;
	for (i = 0; i < K; ++i) 
    {
		while ((!Qi.empty()) && arr[i] >= arr[Qi.back()])

			{ Qi.pop_back(); }

		
		Qi.push_back(i);
	}

	
	for (; i < N; ++i) {

		
		// largest element of the previous window
          ans.push_back(arr[Qi.front()]);
          
		//  Remove the elements which are out of this window
		while ((!Qi.empty()) && Qi.front() <= i - K)
        {
            Qi.pop_front();            
        }

		while ((!Qi.empty()) && arr[i] >= arr[Qi.back()])
        {
            Qi.pop_back();        
        }
			
		Qi.push_back(i);
	}

	// for last window
	ans.push_back(arr[Qi.front()]);

	for(auto i:ans)
    {
        cout<<i<<" ";
    }
}

int main()
{
	int arr[] = { 12, 1, 78, 90, 57, 89, 56 };
	int N = sizeof(arr) / sizeof(arr[0]);
	int K = 3;

	printKMax(arr, N, K);
	return 0;
}
