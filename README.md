# Tic-tac-toe-in-C
This contains the code of tic tac toe in C language.
We can play it but there is also some important codes remaining in this project that will make it looks good...

#include<stdio.h>
#include<conio.h>
#include<stdlib.h>
    int logic(void );
    void asign(char);
    int i,z,j,b[9];
    char m,x,a[]={' ',' ',' ',' ',' ',' ',' ',' ',' '};

 void clrscr();
 void clrscr()
 {
     system("cls");
 }
int main()
{
  clrscr();
  printf(" ___ ___ ___\n|   |   |   |\n| %c | %c | %c |\n|---|---|---|\n| %c | %c | %c |\n|---|---|---|\n| %c | %c | %c |\n|___|___|___|\n\n",a[0],a[1],a[2],a[3],a[4],a[5],a[6],a[7],a[8],a[9]);
  printf("\n First player -> #\n Second player -> O");
  printf("\n\n Win at least 4 rounds out of 7 to win the game.");

//  for(j=0;j<=10;j++)
//{
  for(i=0;i<=8;i++)
  {
   if(i%2==0)
   {
    x='#';
    asign(x);
   }
   else
   {
   x='O';
   asign(x);
   }

    if(i>=4)
    {
      z=logic();
      if(z==1)
      {
       printf(" %c Player won the game  ",x);
       printf("  match end ");
       scanf("%d",&j);

       exit (1);
      }
      else
      {
       if(i==8)
       printf("  Match  tie up... ");
      }
    }

 }
getch();
return 0;
}
 //   Functions  Declarations
int logic()
{
 if(a[0]==x)
 {
 if( a[0]==a[1]&& a[0]==a[2] )
  { // printf(" %c Player  Won the game ",x);
     return 1;
  }
  else if( a[0]==a[3]&& a[0]==a[6] )
  {  return 1;
  }
  else
   if( a[0]==a[4]&& a[0]==a[8] )
   { return 1;
   }
  else
  if( a[1]==a[2]&& a[1]==a[0] )
  {  return 1;
  }
  else
  if( a[1]==a[4]&& a[1]==a[7] )
  {  return 1;
  }
  else
  if( a[2]==a[1]&& a[2]==a[0] )
  {  return 1;
  }
  else
  if( a[2]==a[4]&& a[2]==a[6] )
  {  return 1;
  }
  else
  if( a[2]==a[5]&& a[2]==a[8] )
  {  return 1;
  }
  else
  if( a[3]==a[0]&& a[3]==a[6] )
  {  return 1;
  }
  else
  if( a[3]==a[4]&& a[3]==a[5] )
  {  return 1;
  }
  else
  if( a[6]==a[7]&& a[6]==a[8] )
  {  return 1;
  }
  else
  if( a[6]==a[3]&& a[6]==a[0] )
  {  return 1;
  }
  else
  if( a[6]==a[4]&& a[6]==a[2] )
  {  return 1;
  }
  else
  return 0;
 }
}

void asign(char x)
{
 scanf("%d",&b[i]);
     clrscr();
      if(b[i]==7)
       a[0]=x;
      if(b[i]==8)
       a[1]=x;
      if(b[i]==9)
       a[2]=x;
      if(b[i]==4)
       a[3]=x;
      if(b[i]==5)
       a[4]=x;
      if(b[i]==6)
       a[5]=x;
      if(b[i]==1)
       a[6]=x;
      if(b[i]==2)
       a[7]=x;
       if(b[i]==3)
       a[8]=x;
    printf(" ___ ___ ___\n|   |   |   |\n| %c | %c | %c |\n|---|---|---|\n| %c | %c | %c |\n|---|---|---|\n| %c | %c | %c |\n|___|___|___|\n\n\n",a[0],a[1],a[2],a[3],a[4],a[5],a[6],a[7],a[8]);

}
