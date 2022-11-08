#include <iostream>
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
#include <conio.h>
#include<bits/stdc++.h>
using namespace std;
using std::this_thread::sleep_for;
void output(), judgment(), input(), ended(), rest(),intro(),help(),difficulty();
// st=aawwwwaaaawaaww
// 1=wwaassaawwaawwwaww
// 5=wwwaawwddwwaaaaaaasss
// 3=aawwwwaaaawawww
char m[6][10][10] = {
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 2, 1, 0, 0, 0, 0, 0, 0, 1,
     1, 0, 1, 1, 1, 1, 0, 1, 0, 1,
     1, 0, 0, 0, 1, 0, 0, 1, 0, 1,
     1, 1, 0, 0, 0, 0, 0, 1, 0, 1,
     1, 0, 0, 1, 1, 1, 0, 1, 0, 1,
     1, 0, 0, 0, 0, 1, 0, 0, 0, 1,
     1, 0, 1, 1, 0, 1, 0, 1, 1, 1,
     1, 1, 1, 0, 0, 1, 0, 0, 5, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 2, 1, 0, 0, 0, 0, 0, 0, 1,
     1, 0, 1, 0, 1, 1, 0, 1, 0, 1,
     1, 0, 0, 0, 0, 0, 0, 1, 0, 1,
     1, 1, 0, 1, 1, 1, 1, 1, 1, 1,
     1, 1, 0, 1, 1, 1, 1, 1, 1, 1,
     1, 0, 0, 0, 0, 1, 0, 0, 0, 1,
     1, 0, 1, 1, 0, 1, 0, 1, 0, 1,
     1, 0, 1, 1, 0, 0, 0, 1, 5, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 2, 1, 0, 1, 0, 0, 0, 1, 1,
     1, 0, 1, 0, 0, 0, 1, 0, 1, 1,
     1, 0, 0, 1, 1, 1, 0, 0, 0, 1,
     1, 1, 0, 1, 0, 0, 0, 1, 0, 1,
     1, 0, 0, 0, 0, 1, 1, 1, 0, 1,
     1, 0, 1, 1, 0, 0, 0, 1, 0, 1,
     1, 0, 0, 0, 1, 0, 1, 1, 0, 1,
     1, 1, 1, 0, 1, 0, 0, 0, 5, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 2, 1, 0, 0, 0, 0, 0, 0, 1,
     1, 0, 1, 1, 1, 1, 0, 1, 0, 1,
     1, 0, 0, 0, 1, 1, 0, 1, 1, 1,
     1, 1, 0, 0, 0, 0, 0, 1, 0, 1,
     1, 0, 0, 1, 1, 1, 0, 1, 0, 1,
     1, 0, 0, 0, 0, 1, 0, 0, 0, 1,
     1, 0, 1, 1, 0, 1, 0, 1, 1, 1,
     1, 0, 1, 0, 0, 1, 0, 0, 5, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 2, 0, 0, 0, 0, 1, 0, 0, 1,
     1, 1, 1, 1, 1, 0, 0, 0, 1, 1,
     1, 1, 0, 0, 0, 0, 1, 1, 0, 1,
     1, 0, 0, 1, 1, 0, 0, 0, 0, 1,
     1, 0, 1, 0, 0, 0, 1, 1, 0, 1,
     1, 0, 0, 1, 1, 1, 0, 0, 0, 1,
     1, 1, 0, 1, 0, 0, 0, 1, 1, 1,
     1, 0, 0, 1, 0, 1, 0, 0, 5, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
     1, 0, 0, 0, 0, 0, 0, 0, 0, 1,
     1, 0, 1, 1, 1, 1, 1, 1, 0, 1,
     1, 0, 1, 0, 2, 1, 0, 0, 0, 1,
     1, 0, 0, 0, 1, 1, 0, 1, 1, 1,
     1, 1, 1, 1, 0, 0, 0, 0, 0, 1,
     1, 0, 0, 0, 0, 1, 1, 1, 0, 1,
     1, 0, 1, 0, 0, 1, 1, 1, 0, 1,
     1, 0, 0, 0, 0, 1, 0, 0, 5, 1,
     1, 1, 1, 1, 1, 1, 1, 1, 1, 1}};



char h, ne, pl = '*',st,a;
int k = 8, l = 8, w, x = 1, y = 1, z = 0, t, cnt = 0, ia=10, ja=10,wasd=0,di=0;
void intro()
{
  for(int i=0;i<200000;i++)
  {
        if(i%2==0)
    {
        printf("□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■\n");
        printf("■                                                                                                    □\n");
        printf("□  ▩      ▩    ▩▩▩    ▩▩▩▩▩  ▩▩▩▩▩      ▩▩▩▩    ▩▩▩    ▩      ▩  ▩▩▩▩▩  ■\n");
        printf("■  ▩      ▩  ▩      ▩          ▩  ▩            ▩          ▩      ▩  ▩      ▩  ▩          □\n");
        printf("□  ▩▩  ▩▩  ▩      ▩        ▩    ▩            ▩          ▩      ▩  ▩▩  ▩▩  ▩          ■\n");
        printf("■  ▩  ▩  ▩  ▩▩▩▩▩      ▩      ▩▩▩▩▩    ▩    ▩▩  ▩▩▩▩▩  ▩  ▩  ▩  ▩▩▩▩▩  □\n");
        printf("□  ▩      ▩  ▩      ▩    ▩        ▩            ▩      ▩  ▩      ▩  ▩      ▩  ▩          ■\n");
        printf("■  ▩      ▩  ▩      ▩  ▩          ▩            ▩      ▩  ▩      ▩  ▩      ▩  ▩          □\n");
        printf("□  ▩      ▩  ▩      ▩  ▩▩▩▩▩  ▩▩▩▩▩      ▩▩▩    ▩      ▩  ▩      ▩  ▩▩▩▩▩  ■\n");
        printf("■                                                                                                    □\n");
        printf("□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■\n");
        printf("press space to start\n");
        sleep_for(500ms);
        system("cls");
    }
    else
    {
        printf("■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□\n");
        printf("□                                                                                                    ■\n");
        printf("■  ▩      ▩    ▩▩▩    ▩▩▩▩▩  ▩▩▩▩▩      ▩▩▩▩    ▩▩▩    ▩      ▩  ▩▩▩▩▩  □\n");
        printf("□  ▩      ▩  ▩      ▩          ▩  ▩            ▩          ▩      ▩  ▩      ▩  ▩          ■\n");
        printf("■  ▩▩  ▩▩  ▩      ▩        ▩    ▩            ▩          ▩      ▩  ▩▩  ▩▩  ▩          □\n");
        printf("□  ▩  ▩  ▩  ▩▩▩▩▩      ▩      ▩▩▩▩▩    ▩    ▩▩  ▩▩▩▩▩  ▩  ▩  ▩  ▩▩▩▩▩  ■\n");
        printf("■  ▩      ▩  ▩      ▩    ▩        ▩            ▩      ▩  ▩      ▩  ▩      ▩  ▩          □\n");
        printf("□  ▩      ▩  ▩      ▩  ▩          ▩            ▩      ▩  ▩      ▩  ▩      ▩  ▩          ■\n");
        printf("■  ▩      ▩  ▩      ▩  ▩▩▩▩▩  ▩▩▩▩▩      ▩▩▩    ▩      ▩  ▩      ▩  ▩▩▩▩▩  □\n");
        printf("□                                                                                                    ■\n");
        printf("■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□\n");
        printf("press space to start\n");
        sleep_for(500ms);
        system("cls");
    }

//    a = getchar();
//    if(a=='\n')
//    {
//      break;
//    }
        if(_kbhit())
        {
            if(getch()==' ')
            break;
//            if(getch()=='h' or getch()=='H'){
//                break;
//                sleep_for(500ms);
//                help();
//                sleep_for(500ms);
//                intro();
//            }
        }
    }
}
void difficulty()
{
    system("cls");
    printf("Choose a difficulty\n");
    printf("hard or easy\n");
    printf("easy: press 1 \n");
    printf("hard: press 3 \n");
    std::cin>>di;
    if (di==1)
    {
        wasd=0;
    }
    else if (di==3)
    {
        wasd=1;
    }
}
void help()
{
  system("cls");
  sleep_for(500ms);
  printf("     △   : Up\n");
  printf("   ◁  ▷ : Left / Right\n");
  printf("     ▽   : Down\n");
  printf("   SPACE  : Hard Drop\n");
  printf("     h    : Help\n");
  printf("difficulty: hard or easy\n");
  printf("    g     : difficulty select\n");
  printf("(temporary)\n");
  printf("Enter A to return to the title or game.\n");
}
void input() {
  if (z!=0)
  printf("%d째 맵입니다.\n", t);
  printf("wasd으로\n");
  printf("방향을 입력하시오.\n");
  output();
  for (int i = 0; i < ia; i++) {
    for (int j = 0; j < ja; j++) {
       printf("%c", (char)m[z][i][j]),printf(" ");
    }
    printf("\n");
  }
}
void output() {
  for (int i = 0; i < ia; i++) {
    for (int j = 0; j < ja; j++) {
      if (m[z][i][j] == 0)
        m[z][i][j] = '.'; //빈 공간
      else if (m[z][i][j] == 1)
        m[z][i][j] = '8'; //벽
      else if (m[z][i][j] == 2)
        m[z][i][j] = 'X'; //도착
      else if (m[z][i][j] == 5)
        m[z][i][j] = '*'; //플레이어
    }
  }
}
void judgment(char n) {
  if (n == 'w' or n == 'W') {
    if (m[z][k - 1][l] == '.' || m[z][k - 1][l] == 'X') {
      m[z][k - 1][l] = 5;
      m[z][k][l] = wasd;
      k = k - 1;
      system("cls");
    }

    else {
      m[z][k][l] = 5;
      system("cls");
      printf("벽으로 막혔습니다.\n");
    }

  } else if (n == 'a' or n == 'A') {
    if (m[z][k][l - 1] == '.' or m[z][k][l - 1] == 'X') {
      m[z][k][l - 1] = 5;
      m[z][k][l] = wasd;
      l = l - 1;
      system("cls");

    }

    else {
      m[z][k][l] = 5;
      system("cls");
      printf("벽으로 막혔습니다.\n");
    }
  } else if (n == 's' or n == 'S') {
    if (m[z][k + 1][l] == '.' or m[z][k + 1][l] == 'X') {
      m[z][k + 1][l] = 5;
      m[z][k][l] = wasd;
      k = k + 1;
      system("cls");
    }

    else {
      m[z][k][l] = 5;
      system("cls");
      printf("벽으로 막혔습니다.\n");
    }
  } else if (n == 'd' or n == 'D') {
    if (m[z][k][l + 1] == '.' or m[z][k][l + 1] == 'X') {
      m[z][k][l + 1] = 5;
      m[z][k][l] = wasd;
      l = l + 1;
      system("cls");
    }

    else {
      m[z][k][l] = 5;
      system("cls");
      printf("벽으로 막혔습니다.\n");
    }

  } else if (n == 'h' or n == 'H') {
      help();
  } else if (n == 'g' or n == 'G') {
      difficulty();
    } 
    else {
    system("cls");
    printf("범위을 벗어났습니다\n");
  }
  output();
}
int main() // jhbggjgygujkygygughjvug
{
    intro();
  while (ne != 'E') {
    input();
    ended();
    rest();
  }
}
void ended() {
  while (m[z][x][y] != pl) {
    std::cin >> h;
    judgment(h);
    for (int i = 0; i < ia; i++) {
      for (int j = 0; j < ja; j++) {
        printf("%c", (char)m[z][i][j]),printf(" ");
      }
      printf("\n");
    }
  }
}
void rest() {
  system("cls");
  printf("You won the game!\n");
  printf("if you want a new game,\n");
  printf("Enter 'N' or 'n'\n\n");
  printf("If you want to stop playing,");
  printf("Enter 'E'\n");
  std::cin >> ne;
  if (ne == 'E') {
    printf("close the game");
  } else if (ne == 'n' or ne == 'N') {
    srand(time(NULL));
    printf("%d째 맵입니다.\n", t=rand() % 5+1);//=rand() % 5+1);
    z = t;
    system("cls");
    if (t == 1)
    {
      k = 8, l = 8, pl = '*', x = 1, y = 1;
      m[z][1][1] = 'X',m[z][8][8]='*';
      ia=10, ja=10;
      // 1째맵
    } else if (t == 2)
    {
      k = 8, l = 8, pl = '*', x = 1, y = 1;
      m[z][1][1] = 'X',m[z][8][8]='*';
      ia=10, ja=10;
      // 2째맵
    } else if (t == 3)
    {
      k = 8, l = 8, pl = '*', x = 1, y = 1;
      m[z][1][1] = 'X',m[z][8][8]='*';
      ia=10, ja=10;
      // 3째맵
    } else if (t == 4)
    {
      k = 8, l = 8, pl = '*', x = 1, y = 1;
      m[z][1][1] = 'X',m[z][8][8]='*';
      ia=10, ja=10;
      // 4째맵
    } else if (t == 5)
    {
      pl = '*', x = 3, y = 4, k = 8, l = 8;
      m[5][x][y]=2,m[5][1][1]=0,m[5][8][8]=5;
      ia=10, ja=10;
      // 5째맵
    } else if (t == 6)
    {
      pl = '*', x = 33, y = 60, k = 1, l = 1;
      m[6][x][y]=2,m[6][8][8]=5;
      ia=66, ja=60;
      // 6째맵
    }
  } else {
    rest();
  }
}





/*
□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□
■                                                                                                  ■
□  ▩      ▩    ▩▩▩    ▩▩▩▩▩  ▩▩▩▩▩    ▩▩▩▩    ▩▩▩    ▩      ▩  ▩▩▩▩▩  □
■  ▩      ▩  ▩      ▩          ▩  ▩          ▩          ▩      ▩  ▩      ▩  ▩          ■
□  ▩▩  ▩▩  ▩      ▩        ▩    ▩          ▩          ▩      ▩  ▩▩  ▩▩  ▩          □
■  ▩  ▩  ▩  ▩▩▩▩▩      ▩      ▩▩▩▩▩  ▩    ▩▩  ▩▩▩▩▩  ▩  ▩  ▩  ▩▩▩▩▩  ■
□  ▩      ▩  ▩      ▩    ▩        ▩          ▩      ▩  ▩      ▩  ▩      ▩  ▩          □
■  ▩      ▩  ▩      ▩  ▩          ▩          ▩      ▩  ▩      ▩  ▩      ▩  ▩          ■
□  ▩      ▩  ▩      ▩  ▩▩▩▩▩  ▩▩▩▩▩    ▩▩▩    ▩      ▩  ▩      ▩  ▩▩▩▩▩  □
■                                                                                                  ■
□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□


■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■
□                                                                                                  □
■  ▩      ▩    ▩▩▩    ▩▩▩▩▩  ▩▩▩▩▩    ▩▩▩▩    ▩▩▩    ▩      ▩  ▩▩▩▩▩  ■
□  ▩      ▩  ▩      ▩          ▩  ▩          ▩          ▩      ▩  ▩      ▩  ▩          □
■  ▩▩  ▩▩  ▩      ▩        ▩    ▩          ▩          ▩      ▩  ▩▩  ▩▩  ▩          ■
□  ▩  ▩  ▩  ▩▩▩▩▩      ▩      ▩▩▩▩▩  ▩    ▩▩  ▩▩▩▩▩  ▩  ▩  ▩  ▩▩▩▩▩  □
■  ▩      ▩  ▩      ▩    ▩        ▩          ▩      ▩  ▩      ▩  ▩      ▩  ▩          ■
□  ▩      ▩  ▩      ▩  ▩          ▩          ▩      ▩  ▩      ▩  ▩      ▩  ▩          □
■  ▩      ▩  ▩      ▩  ▩▩▩▩▩  ▩▩▩▩▩    ▩▩▩    ▩      ▩  ▩      ▩  ▩▩▩▩▩  ■
□                                                                                                  □
■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■□■
*/


