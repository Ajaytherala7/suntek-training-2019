# suntek-training-2019
#include<stdio.h> 
#include<string.h>
void main()
{
int i,j,len,k=0; char str[100],rstr[100],vowel[100],consonant[100];
printf("enter the string:\n");
gets(str);
len=strlen(str);
for(i=0;i<len;i++) 
{
if(str[i]=='a' || str[i]=='e' || str[i]=='i' || str[i]=='o' || str[i]=='u' ) 
{
vowel[i]=str[i];
} 
else
{
consonant[k]=str[i];
k++; 
}
}
i=1;
while(str[i]!='\0')
{
if(vowel[i]!='a' || vowel[i]!='e' || vowel[i]!='i' || vowel[i]!='o' || vowel[i]!='u')
{
rstr[i]=consonant[k];
k--; 
}
else
{
rstr[i]=vowel[i]; 
}
printf("%c",rstr[i]);
i++; 
}
}
