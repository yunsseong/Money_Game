#include <stdio.h>
#include <stdlib.h>
#include <time.h>
int main(){
  srand(time(NULL));
  int Input=0;
  int Chance=0;
  int Fullcheck=0;
  int level=0;
  int random=0;
  int Chancelim[3]={9999,60,30};
  bool Boxes[7]={false};
  printf("full the boxes!\n");
  while(level<3&&Chance<Chancelim[level]){
	printf("Your chance is %d\n",Chancelim[level]-Chance); 
	scanf("%d",&Input);
	Chance+=1;
    random = rand()%7;
	Boxes[random]=true;
	for(int i=0;i<7;i++){
		if(Boxes[i]==true){
			printf("*");
			Fullcheck+=1;
		}
		else{
			printf("#");
		}
	}
	printf("\n");
	if(Fullcheck==7){
		printf("You're on the next level");
		Chance=0;
		level+=1;
		for(int i=0;i<7;i++){
			Boxes[i]=false;
		}
		printf("\n");
	}
	Fullcheck=0;
  }
	printf("clear!");
  return 0;
 }
