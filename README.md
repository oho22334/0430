# 0430
## 進階題：最大公因數gcd 
```C
#include <stdio.h>
int main()
{
	int a,b,ans;
	printf("Enter two integers: \n");
	scanf("%d%d",&a,&b);
	if(a>b){
	for(int i=1;i<=b;i++){
		if(a%i==0&&b%i==0)
	ans=i;
	}
	printf("The greatest common divisor of %d and %d is %d\n",a,b,ans);
	}
	else if (a<b){
	for(int i=1;i<=a;i++){
		if(a%i==0&&b%i==0)
		ans=i;
		}
	printf("The greatest common divisor of %d and %d is %d\n",a,b,ans);
		}
		}
```
## 進階題：字串長度 
```C
#include <stdio.h>
#include <string.h>
int main()
{
	char a[100],b[100];
	scanf("%s %s",&a,&b);
	int lena,lenb;
	lena=strlen(a);
	lenb=strlen(b);
	if(lena>lenb) printf("1");
	else if (lenb>lena) printf("-1");
	else{printf("%d",strcmp(a,b));}
	}
```
## 進階題：函數判斷質數
```C
#include <iostream>
using namespace std;
int prime (int n)
{
	int i;
	for(i=2;i<n;i++){
	if(n%i==0)break;
	}
	if(i==n) return 1;
	else return 0;
	}
int main(){
  int n;cin>>n;
  cout<<"["<<prime(n)<<"]";
  return 0;
}
/* 上方 C++ 的 main 函數 等價於 下方 C 的 main 函數
int main(void){
    int n;
    scanf("%d", &n);
    printf("[%d]", prime(n));
    return 0;
}
```
## 進階題：判斷迴文
```C
#include <stdio.h>
#include <string.h>
char a[10000];
int main()
{
	scanf("%s",&a);
	int i;
	int len;
	len=strlen(a);
	for( i=0;i<(len/2);i++){
		if(a[i] !=a[len-1-i])break;
		}
		if( i==(len/2))printf("YES");
		else printf("NO");
		}
```
## 基礎題：計算餘數及列印 
```C
#include <stdio.h>
int main ()
{
	int x,y,temp;
	scanf("%d%d",&x,&y);
	printf("Enter two numbers: The remainder is %d\n",x%y);
	}
```
