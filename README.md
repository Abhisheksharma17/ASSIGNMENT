# ASSIGNMENT Print the LCM and GCD of X and Y.

#include <stdio.h>
long long int lcm(long long int a ,long long int b){
    long long int x;
    x=a*b;
 
    return x;
}
long long int gcd(long long int a ,long long int b){
    long long int x;
    while(b != 0){
    x=b;
    b=a %b;
    a=x;
    }
    return x;
}    
int main()
{
    long long int n;
	scanf("%lld",&n);
	while(n--){
	    long long int a,b;
	    scanf("%lld %lld",&a,&b);
	    long long int y=gcd(a,b);
	    long long int x=lcm(a,b);
	    long long int w=x/y;
	    printf("%lld %lld\n",y,w);
	}
    return 0;
}
 
 
