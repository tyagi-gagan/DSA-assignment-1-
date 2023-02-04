.1=hello world

#include <iostream> 
 #include <cstdio> 
 using namespace std; 
  
 int main() { 
     printf("Hello, World!"); 
     return 0; 
 }
  
 .2=input or output
  
  include<iostream> 
 using namespace std; 
 int main() 
 { 
         int a,b,c; 
          
         cin>>a>>b>>c; 
          
         cout<<(a+b+c); 
         return 0;         
 }
  
  
 .3=data types
  
  include <iostream> 
 #include <cstdio> 
 using namespace std; 
  
 int main() { 
     int i; 
     long l; 
     char c; 
     float f; 
     double d; 
      cin >>i >>l >> c>> f >>d; 
         
      printf("%d\n%ld\n%c\n%.3f\n%.9lf\n", i, l, c,f,d); 
  
     return 0; 
 }
  
 .4=function
  
  #include <iostream> 
 #include <cstdio> 
 using namespace std; 
  
 int max_of_four(int a,int b,int c,int d) 
 { 
     if(a>b&& a>c && a>d){ 
         return (a); 
     } 
     else if (b>a&& b>c&& b>d){ 
     return (b);     
     } 
     else if(c>a&& c>b&& c>d){ 
         return (c); 
     } 
     else { 
         return (d); 
     } 
     } 
     int main() 
     { 
     int a,b,c,d; 
     scanf("%d %d %d %d", &a,&b,&c,&d); 
     int ans = max_of_four(a,b,c,d); 
     printf("%d",ans); 
       
      return 0; 
      
     }
  
  .5=loops
  
  #include <iostream> 
 #include <cstdio> 
 using namespace std; 
 int main() { 
     // Complete the code. 
     int a, b; 
     cin >> a >> b; 
     for (int i = a; i<=b; i++) 
     { 
         if ( i == 1){ 
             cout << "one" << endl; 
         } 
         else if ( i == 2) { 
             cout << "two" << endl; 
         } 
         else if ( i == 3){ 
             cout << "three" << endl; 
         } 
         else if ( i == 4) { 
             cout << "four" << endl; 
         } 
         else if ( i == 5) { 
             cout << "five" << endl; 
         } 
         else if ( i == 6) { 
             cout << "six" << endl; 
         } 
         else if ( i == 7) { 
             cout << "seven" << endl; 
         } 
         else if ( i == 8) { 
             cout << "eight" << endl;   
         } 
         else if ( i == 9) { 
             cout << "nine" << endl;  
         } 
         else if ( i > 9) { 
             if ( i % 2 == 0) { 
             cout << "even" << endl; 
             } 
             else { 
             cout << "odd" <<endl; 
             } 
         }          
     } 
      
     return 0; 
 }
  
  .6=pointer
  
  #include <stdio.h> 
 void update(int *a,int *b) { 
     // Complete this function  
     int temp = *a;    
     *a = *a + *b; 
     *b = temp - *b; 
      
     if (*b < 0) 
     { 
         *b = -(*b); 
     } 
 } 
 int main() { 
     int a, b; 
     int *pa = &a, *pb = &b; 
      
     scanf("%d %d", &a, &b); 
     update(pa, pb); 
     printf("%d\n%d", a, b); 
     return 0; 
 }
                
.7=strings               
                
  #include <iostream> 
 #include <string> 
 using namespace std; 
 int main() { 
     // Complete the program 
     string a,b; 
     cin >> a >> b ; 
     int l_of_a = a.size(); 
     int l_of_b = b.size(); 
     cout << l_of_a <<" "<<l_of_b << endl; 
     cout << a << b << endl; 
     char c1 = a[0]; 
     char c2 = b[0]; 
     a[0] = c2; 
     b[0] = c1; 
     cout << a <<" "<<b; 
     return 0; 
     {
   
 .8=Array reversal
  
  #include<iostream> 
  
 using namespace std; 
  
 int main() 
 {  
     int n; 
  
     int arr[1000]; 
  
     cin>>n; 
  
     for(int i=0;i<n;i++) 
  
     { 
  
         cin>>arr[i]; 
  
     } 
  
     for(int i=0;i<n/2;i++) 
  
     { 
  
         int temp; 
  
         temp=arr[i]; 
  
         arr[i]=arr[n-1-i]; 
  
         arr[n-1-i]=temp; 
  
     } 
  
     for(int i=0;i<n;i++) 
  
     { 
  
         cout<<arr[i]<<" "; 
  
     } 
     return 0; 
 }
