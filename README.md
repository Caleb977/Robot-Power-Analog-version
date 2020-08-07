#include<stdio.h>
int main(){
    int NumberOfRobot;
    int EnginePower;
    int Resistance;
    int Weight;
    int Height;
    int TotalPower;
    int GeneralPower = 0;
    int i;
    scanf("%d",&NumberOfRobot);
    
    for(i=0; i<NumberOfRobot; i++){
         scanf("%d%d%d%d",&Height,&Weight,&EnginePower,&Resistance);
         
         TotalPower = (EnginePower+Resistance)*(Weight-Height);
         
         GeneralPower = GeneralPower + TotalPower; 
    }
    
    printf("%d",GeneralPower);
 return 0;
    
}
