# main-menu
#include <stdio.h>
#include <stdlib.h>
int i,k;
void start();
char op;
int main()
{
start();
}
void start(){
   /// XML();
    int choose;
    system("cls");                              //CLEAR SCREEN AFTER EACH PLAY
    for(i=0;i<15;i++)printf("\n");
    system("COLOR 1C");                         //CHANGING THE COLOR OF SCREEN
    printf("                              Welcome to connect four\n");              //WELCOME MESSAGE
    Sleep(1000);///--->?
    for(k=0;k<3;k++)printf("\n");
    system("COLOR EC");                           //CHANGING COLR OF THE SCREEN
    printf("                                   1-new game\n"                ////////////////////////////
           "                                   ----------  \n"              //                          //
          "                                   2-high scores\n"              //    MAIN MENU            //
          "                                   -------------\n"              ////////////////////////////
          "                                   3-load game\n"
          "                                   -----------\n"
          "                                   4-instruction\n"
          "                                   -------------     \n "
          "                                  5-exit           \n "
         "                                   -------------       "
          "                                   \n");
    printf("choose from the previous options: \n");
    for(i=0;i<32;i++)printf("-");                                              //SCAN THE OPERATION TYPE FROM THE USER
    printf("\n");
    scanf("%d",&choose);         //GET THE USER CHOOSE
    if(choose==5)
    {printf("are you sure to exit y/n: ");
        scanf("%ch",&op);///----->to read character %ch///

        if(op=='y')
            exit(1);///----->??
        else start() ;
    }
    else{
    switch(choose){
       // case 1: //printnumber();break;
        //case 2: High_Score();break;
        //ase 3: read[0]='l';save_load();printnumber();break;
        //case 4: instrctions();break;

                    //start();}

        default: printf("error please try again !!");
}}
}
