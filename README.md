#include<bits/stdc++.h>
using namespace std;

typedef long long ll;
typedef double dl;

#define endl "\n"
#define optimize() ios_base::sync_with_stdio(0);cin.tie(0);cout.tie(0);
#define fraction() cout.unsetf(ios::floatfield); cout.precision(10); cout.setf(ios::fixed,ios::floatfield);
#define mem(a,b) memset(a, b, sizeof(a))

int main()
{
    optimize();
    stack<int> st;

    int t;
    cin >> t;
    string s;

    while(t--)
    {
        cin >> s;
        if(s=="push")
        {
            int x;
            cin >> x;
            st.push(x);
        }

        else if(s=="pop")
        {
            if(!st.empty())
            {
                cout << st.top() << endl;
                st.pop();
            }
            else
            {
                cout << "Empty" << endl;
            }
        }

    }
}
