```cpp
#include <bits/stdc++.h>
using namespace std;
///-----Policy Based DS-----///
#include <ext/pb_ds/assoc_container.hpp>
#include <ext/pb_ds/tree_policy.hpp>
using namespace __gnu_pbds; //we'll extract more DS frim here soon

///-----Frequent Expressions-----///
// Basic
#define pb push_back
#define fi first
#define se second
#define mp make_pair
#define sz(x) (int)((x).size())
#define all(x) (x).begin(),(x).end()
// In/0ut
#define FastIO ios::sync_with_stdio(false);cin.tie(0);cout.tie(0)
#define nl "\n"
#define YES cout<<"YES"<<nl
#define NO cout<<"NO"<<nl
#define yes cout<<"yes"<<nl
#define no cout<<"no"<<nl
#define Yes cout<<"Yes"<<nl
#define No cout<<"No"<<nl
// I/0 part 2
template <typename Fi, typename Se> ostream& operator<<(ostream& os, pair<Fi,Se> x){os << '(' << x.fi << ',' << x.se << ')';return os;}
template <typename Fi, typename Se> istream& operator>>(istream& in, pair<Fi,Se> x){in >> x.fi >> x.se;return in;}
template <typename T> ostream& operator<<(ostream& os, vector<T> v){for(const auto& x : v)os << x << ' ';return os;}
// I/0 part 3
void args_out(ostream& os){ os << nl; }
template <typename Head, typename... Tail> void args_out(ostream& os, Head H, Tail... T){os << H << ' ' ;args_out(os, T...);}
#define print(...) args_out(cout, __VA_ARGS__)
// DebuGGing
#define dbg(...) cerr << "--->(" << #__VA_ARGS__ << ") :\n", args_out(cerr, __VA_ARGS__);
#define dbgv(v, n) cerr << #v << " : " << "\n"; for(int i = 0; i < n; i++) cerr << "\t" << #v << "[" <<  i <<  "]" <<  " : " << v[i] << "\n"; cerr << nl;
#define sep() cerr << "--------------------" << nl;
// L00Ps
#define REP(i,n) for(int i = 0 ; i < (n) ; i++)
#define RREP(i,n) for(int i = (n-1) ; i > -1 ; i--)
#define FOR(i,a,b) for (int i = (a); i < (b); i++)
#define FORI(i,a,b) for (int i = (a); i <= (b); i++)
#define RFOR(i,b,a) for (int i = (b) - 1; i >= (a); i--)
#define GO(s,iter) for(auto& iter=(s).begin(); iter!=(s).end(); iter++) // forgot about u my friend 
// T-ai-pss
typedef long long ll;
typedef unsigned long long ull;
typedef pair<int, int> pii;
typedef vector<int> vi;
typedef vector<vi> vvi;
typedef vector<pii> vii;
// Money
const ll mod = 1e9 + 7; //Update for each pb, sometimes : 998244353
const ll inf = 1e18;
mt19937_64 mt(chrono::steady_clock::now().time_since_epoch().count());
// Short Data Structures        (p_q)(q_p)
template<typename T> using ordered_set = tree<T,null_type,less<T>,rb_tree_tag,tree_order_statistics_node_update>; // aka indexed_set
// Graph                        (T_T)(o_o)
int dx[4]={1,0,-1,0},dy[4]={0,1,0,-1}; //East-North-West-South
// Number Theory                (>_<)(^o^)
ll gcd(ll a, ll b){while(b){swap(a,b);b%=a;}return(a);}
ll lcm(ll a, ll b){return (a*b)/gcd(a, b);}
ll po2(ll b,ll e){if(e==0)return 1; ll res = 1;while(e>1){if(e%2)res=(res*b)%mod;e/=2;b=(b*b)%mod;}return(res*b)%mod;}
ll modInverse(ll a){ return po2(a, mod-2); }
// Long Long Wrapper            (@_@)(°_°)
struct LL{ll v;LL(){}LL(ll x):v(x%mod){}LL(int x):v(x%mod){}};
LL operator*(LL x, LL y){return LL((x.v*y.v)%mod);}LL operator*(LL x, ll y){return LL((x.v*y)%mod);}
LL operator+(LL x, LL y){return LL((x.v+y.v)%mod);}LL operator+(LL x, ll y){return LL((x.v+y)%mod);}
LL operator-(LL x, LL y){return LL((x.v-y.v)%mod);}LL operator-(LL x, ll y){return LL((x.v-y)%mod);}
LL operator^(LL x, LL y){return LL(po2(x.v,y.v));}
LL pos(LL x){return x.v < 0 ? LL(x.v + mod): x ;}
ostream& operator<<(ostream& os, LL x){return os << x.v;}
istream& operator>>(istream& in, LL x){return in >> x.v;}
// Combinatorics                (-_-)(^_^)(._.) 
/*
const int maxn = (int)2e5 + 1; // (^-^)Update me pls(.^.)
LL fact[maxn], invf[maxn];
LL P(int n){return fact[n];}
LL A(int n, int k){return fact[n]*invf[n-k];}
LL C(int n, int k){return fact[n]*invf[n-k]*invf[k];}
void preprocess(){
    //call me once at the start of main (0_0)(;_;)
    fact[0] = 1;
    FOR(i,1,maxn)
        fact[i] = fact[i-1] * i;
    invf[maxn-1].v = modInverse(fact[maxn-1].v);
    RFOR(i,maxn-1,0)
        invf[i] = invf[i+1] * (i+1);
}
*/

void solve()
{
    
}

int main()
{
    auto start = chrono::high_resolution_clock::now();
    FastIO;
    //Preprocessing here please...
    int t = 1 ;
    cin >> t;//press `Tab` to go to solve
    while(t--)
        solve();
    auto end = chrono::high_resolution_clock::now();
    chrono::duration<double> duration;
    duration = end - start;
    cerr << "\n\t"<< duration.count() << 's' << endl;
    return 0;
}
```