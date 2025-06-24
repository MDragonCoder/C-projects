#include <cstddef>

typedef int Die;// complex int element declaration - flexible
int rollDice(Die *d1, Die *d2);// points towards the memory location of d1 and d2

int main(void){// creates the test format for rollDie
    srand(time(NULL));// time is
    Die d1 = 4, d2 = 4;// DECLARATIONS OF THE FIRST ROLL
    int totalR = 0;
    int rollSum = 0;
    int sevEle = 0;
    while (rollSum!=12){
        rollSum = rollDice(&d1, &d2);// stores result of function
        printf("(%d,%d)\n",d1,d2);// prints 
        if(rollSum ==7 || rollSum == 11){
            sevEle++;
        totalR++;
        }
    }
    printf("%d total rolls & %d seven or eleven\n",totalR,sevEle);
    return 0;
}
int rollDice(Die *d1, Die*d2){// supplies results to main
    *d1 = rand()%6+1;// makes random roll
    *d2 = rand()%6+1; // makes random roll
    return (*d1 + *d2);
}

