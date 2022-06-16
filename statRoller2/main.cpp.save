#include <iostream>
#include <stdlib.h>
#include <time.h>
#include <algorithm>

using namespace std;

int statGen()
{
    int stat = 0;
    //Generates the random numbers for the dice rolls
    int die1 = 1+ (rand()%6);
    int die2 = 1+ (rand()%6);
    int die3 = 1+ (rand()%6);
    int die4 = 1+ (rand()%6);
    //Finds and eliminates the lowest roll
    int rolls[4] = {die1, die2, die3, die4};
    sort(rolls, rolls+4);
    rolls[0] = 0;
    //Adds the 3 highest rolls together and returns the result
    for(int i = 0; i<4; i++){
        stat+=rolls[i];
    }
    return stat;
}

int main()
{
    srand(time(NULL));
    //Runs the function to generate a stat 6 times and outputs the results
    for(int i = 0; i<6; i++){
        cout<<statGen()<<endl;
    }
    system("pause");
    return 0;
}
