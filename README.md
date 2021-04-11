# Electric-Bill

#include<stdio.h>

int main()
{ //FUNCTIONS 
    int id, b, u;
    double s, t;
    // USERS INPUTS
    printf("Consumer id: ");
    scanf("%d", &id);
    printf("Consumed Unit: ");
    scanf("%d", &u);
    
    printf("\n\nCustomer ID number: %d", id);
    // IDENTIFYING THE UNIT AND CHARGES
    if(u<250)
    {
    printf("\nPrice of unit in Peso: P1.50");
    b=u*1.50; //Calculating the bill
    printf("\nPartial Bill: P%d", b);
    s=b*0.1; //Calculating the surcharge
    printf("\nSurcharge: P%f", s);
    t=b+s; // getting the total
    printf("\nTotal Bill: P%f", t);
    }else if(u>=250, u<=449)
    {
    printf("\nPrice of unit in Peso: P1.60");
    b=u*1.60; //Calculating the bill
    printf("\nPartial Bill: P%d", b);
    s=b*0.1;
    printf("\nSurcharge: P%f", s);
    t=b+s;
    printf("\nTotal Bill: P%f", t);
    }else if(u>=450, u<=599)
    {
    printf("\nPrice of unit in Peso: P1.85");
    b=u*1.85; //Calculating the bill
    printf("\nPartial Bill: P%d", b);
    s=b*0.1;
    printf("\nSurcharge: P%f", s);
    t=b+s;
    printf("\nTotal Bill: P%f", t);
    }else if(u>=600)
    {
    printf("\nPrice of unit in Peso: P2");
    b=u*2; //Calculating the bill
    printf("\nPartial Bill: P%d", b);
    s=b*0.1;
    printf("\nSurcharge: P%f", s);
    t=b+s;
    printf("\nTotal Bill: P%f", t);
    }
    return 0;
}
