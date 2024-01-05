# ordered_Multiset


#include <iostream> 
using namespace std; 

#include <ext/pb_ds/assoc_container.hpp> 
#include <ext/pb_ds/tree_policy.hpp> 
using namespace __gnu_pbds; 

#define ordered_set tree<int, null_type,less_equal<int>, rb_tree_tag,tree_order_statistics_node_update> 

// <---  to erase one occurrence of some value from the set we can write " s.erase(s.upper_bound(value)) "  ---> // 

int main() 
{ 
int t=1;
while(t--){

ordered_set st;
st.insert(1);

st.insert(1);
cout<<st.size();

st.erase(st.upper_bound(1));


}

	return 0; 
} 
