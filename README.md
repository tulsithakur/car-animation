# car-animation

#include<iostream.h>
#include<conio.h>
#include<graphics.h>
#include<dos.h>
void main()
{
clrscr();
int gd=0, gm;


initgraph(&gd, &gm, "C:\TC\BGI");

cout<<"\n\n\n\n\nMade By: TULSI THAKUR\n\n\n\n\n\n\n\n";


//***ROAD***//
for(int i=0;i<620;i++)
{

//***CAR's BODY***//
line(0,400,900,400);

circle(150+i,379,20);    //first wheel
circle(350+i,379,20);    //second wheel
circle(150+i,379,5);
circle(350+i,379,5);
arc(150+i,380,0,180,22);
arc(350+i,380,0,180,22);
line(172+i,380,328+i,380);
line(128+i,380,50+i,380);
line(50+i,380,50+i,320);
line(50+i,320,128+i,320);
line(128+i,320,170+i,280);
line(170+i,280,290+i,280);
line(290+i,280,345+i,320);
line(372+i,380,450+i,380);
line(450+i,380,450+i,320);
line(345+i,320,450+i,320);

line(180+i,300,220+i,300); //first window
line(180+i,300,180+i,335);
line(220+i,300,220+i,335);
line(180+i,335,220+i,335);

line(250+i,300,290+i,300);//second window
line(250+i,300,250+i,335);
line(290+i,300,290+i,335);
line(250+i,335,290+i,335);

 delay(10);
 cleardevice();
 }
cout<<"\n\n\t\t\t\tMade by: Tulsi Thakur\n\n\n\t";
cout<<"\n\n\t\t\t\t(Press Enter)\n\n\n\t";
getch();
closegraph();
}
