# Functions-in-C
In this challenge, you will learn simple usage of functions in C. Functions are a bunch of statements glued together. A function is provided with zero or more arguments, and it executes the statements on it. Based on the return type, it either returns nothing (void) or something.
#include <stdio.h>

int max_of_four(int w,int x,int y,int z){
    if(w>x && w>y && w>z){
        return w;
    }
    else if(x>w && x>y && x>z){
        return x;
    }
    else if(y>x && y>w && y>z){
        return y;
    }
    else if(z>x && z>y && z>w){
        return z;
    }
    return 0;
}
int main() {
    int a, b, c, d;
    scanf("%d %d %d %d", &a, &b, &c, &d);
    int ans = max_of_four(a, b, c, d);
    printf("%d", ans);
    
    return 0;
}
