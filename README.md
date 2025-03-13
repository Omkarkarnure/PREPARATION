# PREPARATION
/* You are given an array arr of size n - 1 that contains distinct integers in the range from 1 to n (inclusive). This array represents a permutation of the integers from 1 to n with one element missing. Your task is to identify and return the missing element.*/
//{ Driver Code Starts
#include <bits/stdc++.h>
using namespace std;


// } Driver Code Ends

// User function template for C++
class Solution {
  public:
    int missingNumber(vector<int>& arr) {
        // code here
    }
};


//{ Driver Code Starts.

int main() {
    int t;
    cin >> t;
    cin.ignore(); // to ignore the newline after the integer input
    while (t--) {
        int n;
        vector<int> a;
        string input;

        // Input format: first number n followed by the array elements
        getline(cin, input);
        stringstream ss(input);
        int num;
        while (ss >> num)
            a.push_back(num);

        Solution obj;
        cout << obj.missingNumber(a) << endl;
        cout << "~\n";
    }

    return 0;
}

// } Driver Code Ends
/* User function template for C++
class Solution {
  public:
    int missingNumber(vector<int>& arr) {
        int n = arr.size();
        vector<int>  hash(n+1, 0);
        for(int i=0; i<n; i++){
            if(arr[i]>0 && arr[i]<=n){
                hash[arr[i]]++;
            }
            
        }
        for(int i=1; i<=n; i++){
            if(hash[i]==0) return i;
        }
        return n+1;
        // code here
    }*/
};
