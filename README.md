<div align="center">

## Customizable Menu Uses the arrow keys and return keys


</div>

### Description

Need A Cool Menu? Here you go. You can change the text and highlight color in seconds. Though not commented very well it is easy to see what is happining. Made by a begginer for expert programs

Please email me and tell me what you think!!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[theMayor](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/themayor.md)
**Level**          |Beginner
**User Rating**    |3.7 (11 globes from 3 users)
**Compatibility**  |C\+\+ \(general\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/themayor-customizable-menu-uses-the-arrow-keys-and-return-keys__3-1871/archive/master.zip)





### Source Code

```
#include <iostream.h>
#include <conio.h>
#include <stdlib.h>
//**********************************************
int color=10;  // Change the number to change the text color
int highlight=14; // Change the number to change the text color
int choice=8;
void options()
{
 system ("cls");
 if (choice==8)
 {
 cout << "You Chose New Game!!!\n";
 // your code goes here
 }
 else if (choice==9)
 {
  cout << "You Chose To Highscores!!\n";
  // your code goes here
 }
}
//*********************************************************************************************
//Do not edit Below This line
//*******************************************************************************************
void menu()
{
 textcolor(color);
 gotoxy(35,8);
 textbackground(0);
 if (choice==8)
 {
 textbackground(highlight);
 }
 cprintf("New Game");
 gotoxy(35,9);
 textbackground(0);
 if (choice==9)
 {
 textbackground(highlight);
 }
 cprintf ("High Scores");
 gotoxy(35,10);
 textbackground(0);
 if (choice==10)
 {
 textbackground(highlight);
 }
 cprintf ("Exit");
 cout <<endl;
}
int main()
{
 system ("cls");
 menu();
 char key;
 for (;;)
 {
 key=getch();
 if (key=='\r')
 {
 options();
 break;
 }
 switch (key)
 {
  case 'H':
  if (choice-1<8)
  {
  break;
  }
  else
  {
  choice--;
  }
  menu();
  break;
  case 'P':
  if (choice+1>10)
  {
  break;
  }
  else
  {
  choice++;
  }
  menu();
  break;
 }
 }
 return 0;
}
```

