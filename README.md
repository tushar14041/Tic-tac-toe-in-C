#include<stdio.h>
#include<conio.h>
#include<stdlib.h>
//#include<windows.h>
    int logic(int );
    int asign(char);
    int n,i,z,j,k,b[9];
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
  printf("\n First player  -> X\n Second player -> O");
//  printf("\n\n Win at least 4 rounds out of 7 to win the game.\nenter first move and Start the game\n");

  for(i=0;i<=8;i++)
  {
   if(i%2==0)
   {
    x='X';
    n = asign(x);
    printf(" ___ ___ ___\n|   |   |   |\n| %c | %c | %c |\n|---|---|---|\n| %c | %c | %c |\n|---|---|---|\n| %c | %c | %c |\n|___|___|___|\n\n\n",a[0],a[1],a[2],a[3],a[4],a[5],a[6],a[7],a[8]);
   }
   else
   {
    x='O';
    n = asign(x);
    printf(" ___ ___ ___\n|   |   |   |\n| %c | %c | %c |\n|---|---|---|\n| %c | %c | %c |\n|---|---|---|\n| %c | %c | %c |\n|___|___|___|\n\n\n",a[0],a[1],a[2],a[3],a[4],a[5],a[6],a[7],a[8]);
   }

   if(i>=4)
   {
    z=logic(n);
    if(z==1)
    {
     if(i%2==0)
     {

    printf( " ______   __      __        __   _______   ____      __    ____    \n");
    printf( "|  __  | /  \\    |  |      |  | |__   __| |    \\    |  |  |    |   \n");
    printf( "| |__| ||_  |    |  |  __  |  |    | |    |     \\   |  |  |    |   \n");
    printf( "|  ____|  | |    |  | /  \\ |  |    | |    |  |\\  \\  |  |  |    |   \n");
    printf( "| |       | |    |  |/ /\\ \\|  |    | |    |  | \\  \\ |  |  \\    /   \n");
    printf( "| |     __| |__  |    /  \\    |  __| |__  |  |  \\  \\|  |   \\  /    \n");
    printf( "|_|    |_______|  \\__/    \\__/  |_______| |__|   \\_____|    \\/     \n");
    printf( "                                                             _     \n");
    printf( "                                                            |_|    \n");


      printf(" 1st Player won the game  ",x);

            scanf("  match end ! press any key to exit. ",&k);
     exit (1);

      }
    else
    {
    printf(" ______    ____       __        __   _______   ____      __    ____    \n");
    printf("|  __  |  / _  \\     |  |      |  | |__   __| |    \\    |  |  |    |   \n");
    printf("| |__| | |_/ \\  |    |  |  __  |  |    | |    |     \\   |  |  |    |   \n");
    printf("|  ____|     |  |    |  | /  \\ |  |    | |    |  |\\  \\  |  |  |    |   \n");
    printf("| |         /  /     |  |/ /\\ \\|  |    | |    |  | \\  \\ |  |  \\    /   \n");
    printf("| |        /  /___   |    /  \\    |  __| |__  |  |  \\  \\|  |   \\  /    \n");
    printf("|_|       /_______|  \\___/    \\__/  |_______| |__|   \\_____|    \\/     \n");
    printf(  "                                                                 _     \n");
    printf(  "                                                                |_|    \n");

           printf("2nd Player won the game  ",x);
            scanf("  match end ! press any key to exit. ",&k);

    exit (1);
       }
      }
    else
       {
        continue;
       }

    }

 }
  printf(" ______      _____       ____        __      __     ____             \n");
  printf("|  __  \\    |  _  \\     /  _ \\      |  |    |  |   |    |        \n");
  printf("| |  |  \\   | |_| |    |  |_| |     |  |    |  |   |    |         \n");
  printf("| |  |   |  |    /     |      |     |  | __ |  |   |    |      \n");
  printf("| |__|   /  | |\\ \\     |  /\\  |     |  |/  \\|  |   \\    /                 \n");
  printf("|       /   | | \\ \\    | |  | |     |    /\\    |    \\  /               \n");
  printf("|______/    |_|  \\_\\   |_|  |_|     \\___/  \\___/     \\/        \n");
  printf("                                                                   \n");
  printf("                                                      _                \n");
  printf("                                                     |_|                 \n");
  printf("                                                                          \n");


            scanf("  match end ! press any key to exit. ",&k);
 exit(0);

getch();
return 0;
}
 //   Functions  Declarations


int logic(int n)
{

 int r=0;
 switch(n)
 {

 case 0:
 {
  if( a[0]==a[1]&& a[0]==a[2] )
  {  r=1;
  }
  else
  if( a[0]==a[3]&& a[0]==a[6] )
  {  r=1;
  }
  else
  if( a[0]==a[4]&& a[0]==a[8] )
   { r=1;
   }
   break;
 }

 case 1:
 {
  if( a[1]==a[2]&& a[1]==a[0] )
  {  r=1;
  }
  else
  if( a[1]==a[4]&& a[1]==a[7] )
  {  r=1;
  }
  break;
 }

 case 2:
 {
  if( a[2]==a[1]&& a[2]==a[0] )
  {  r=1;
  }
  else
  if( a[2]==a[4]&& a[2]==a[6] )
  {  r=1;
  }
  else
  if( a[2]==a[5]&& a[2]==a[8] )
  {  r=1;
  }
  break;
 }

 case 3:
 {
  if( a[3]==a[0]&& a[3]==a[6] )
  {  r=1;
  }else
  if( a[3]==a[4]&& a[3]==a[5] )
  {  r=1;
  }
  break;
 }
 case 4:
 {
  if( a[0]==a[4]&& a[0]==a[8] )
  { r=1;
  }
  else
  if( a[1]==a[4]&& a[1]==a[7] )
  {  r=1;
  }
  else
  if( a[2]==a[4]&& a[2]==a[6] )
  {  r=1;
  }
  else
  if( a[3]==a[4]&& a[3]==a[5] )
  {  r=1;
  }
  break;
}
 case 5:
 {
  if( a[2]==a[5]&& a[2]==a[8] )
  {  r=1;
  }
  else
  if( a[3]==a[4]&& a[3]==a[5] )
  {  r=1;
  }
  break;
}
 case 6:
 {
  if( a[6]==a[7]&& a[6]==a[8] )
  {  r=1;
  }
  else
  if( a[6]==a[3]&& a[6]==a[0] )
  {  r=1;
  }
  else
  if( a[6]==a[4]&& a[6]==a[2] )
  {  r=1;
  }
  break;
}
 case 7:
 {
  if( a[1]==a[4]&& a[1]==a[7] )
  {  r=1;
  }
  else
  if( a[6]==a[7]&& a[6]==a[8] )
  {  r=1;
  }
  break;
 }
  case 8:
{
  if( a[2]==a[5]&& a[2]==a[8] )
  {  r=1;
  }
  else
  if( a[0]==a[4]&& a[0]==a[8] )
   { r=1;
   }
  else
  if( a[6]==a[7]&& a[6]==a[8] )
  {  r=1;
  }
  break;
}

default:
 {  printf("This is default section : ");
   break ;
 }

}
return r;

}


int asign(char x)
{
    printf("\nTurn of : %c = ",x);
    scanf("%d",&b[i]);
     clrscr();
      if(b[i]==7)
       { a[0]=x;
         return 0; }
      if(b[i]==8)
       { a[1]=x;
         return 1; }
      if(b[i]==9)
       { a[2]=x;
         return 2; }
      if(b[i]==4)
       { a[3]=x;
         return 3; }
      if(b[i]==5)
       { a[4]=x;
         return 4; }
      if(b[i]==6)
       { a[5]=x;
         return 5; }
      if(b[i]==1)
       { a[6]=x;
         return 6; }
      if(b[i]==2)
       { a[7]=x;
         return 7; }
      if(b[i]==3)
       { a[8]=x;
         return 8;  }

}


7
8
