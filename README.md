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
