# java笔试编程题
## java实现字符串的逆序

```
public static String reverse(String s){
char[] chars=s.toCharArray();
int i;
s="";
for(i=chars.length-1;i>=0;i--)
s+=chars[i];
return s;
}

```
## 求编写JAVA螺旋矩阵
```
public class N {
 public static void main(String[] args) {
  final int N=4;
  int a[][]=new int[N][N];
  int num=1;
  int i=0,j=0,m=0;
  if(N%2==0) 
   m=N/2; 
  else 
   m=N/2+1; 
  for(i=0;i<=m-1;i++){  
   for(j=i;j<=N-i-1;j++){
    a[i][j]=num;
    num++;
   } 
   for(j=i+1;j<=N-i-1;j++) {
    a[j][N-i-1]=num;
    num++;
   }  
   for(j=N-i-2;j>=i;j--){
    a[N-i-1][j]=num;
    num++;
   } 
   for(j=N-i-2;j>=i+1;j--){
    a[j][i]=num;
    num++;
   } 
  } 
  for(i=0;i<N;i++){
   for(j=0;j<N;j++){
    System.out.print(String.format("%3d",a[i][j]));
   }
   System.out.println();
  }
 }
}
```
