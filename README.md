#include<stdio.h>
#include<conio.h>
#include<stdlib.h>
#include<string.h>
int main()
{
    int u,d,r,l,nod, compare;
    char name[100],phno[10];
    char city[100], vno[100];
    char cnf[20];
    printf("Name of the Customer : \n");
    scanf("%s", name);
    printf("Place of the Customer :\n");
    scanf("%s", city);
    printf("Enter the ph no :\n");
    scanf("%s", phno);
    printf("Enter the no of days : \n");
    scanf("%d", &nod);
    printf("Enter the hired Vehicle Reg No : \n");
    scanf("%s", &vno);
    rental:
        printf("\n CAR RENTAL APPLICATION \n");
        printf("\n ----------------------- \n");
        printf("\n Press 1 for Deluxe Vehicles \n");
        printf("\n Press 2 for Seven seater Vehicles \n");
        printf("\n Press 3 for Luxury Vehicle \n");
        printf("\n ---------------------------- \n");
        printf("\n Press any Option: \n");
        scanf("%d", &u);
        switch(u)
        {
            case 1:
                printf("\n You have chosen Deluxe Vehicles \n");
                printf("\n Deluxe Vehicle Available are \n");
                printf("\n Maruti SWIFT, I20, V.POLO, Amaze \n");
                printf("\n ------------------------------ \n");
                printf("\n do u want to hire, Press 1 for SWIFT, 2 for I20, 3 for POLO, 4 for Amaze\n");
                scanf("%d", &d);
                switch(d)
                {
                    case 1:
                    printf("\n You have selected SWIFT includes fuel cost also | %ldrs per day \n ie total %ldRs\n",10000/nod,10000);
                    break;

                    case 2:
                    printf("\n You have selected I20 includes fuel cost also|%ldrs per day \n ie total %ldRs\n",15000/nod,15000);
                    break;

                    case 3:
                    printf("\n You have selected Volkswagen Polo includes fuel cost also| %ldrs per day \n ie total %ldRs\n",17000/nod,17000);
                    break;

                    case 4:
                    printf("\n You have selected Amaze includes fuel cost also| %1drs per day \n ie total %1dRs\n",20000/nod,20000);
                    break;

                    default:
                    printf("You have chosen wrong option\n");
                    break;
                }
    printf("Name of the customer : %s \n",name);
    printf("Place of Hiring : %s \n",city);
    printf("Contact number of the Customer is : %s \n",phno);
    printf("Number of days Vehicle is hired : %d \n",nod);
    printf("Registeration number of the hired vehicle : %s \n",vno);
    printf("are you want to confirm the booking\n Yes \n No\n");
    scanf("%s",&cnf);
    compare = strcmp(cnf,"yes");
    if(compare==0){
        break;
    }
    else{
     goto rental;
    }

            case 2:
            printf("\n You have chosen Seven seater Vehicles \n");
            printf("\n Vehicles Available are \n");
            printf("\n TATA SUMO, TAVERA, TOOFAN, INNOVA \n");
            printf("\n ----------------------------- \n");
            printf("\n do u want to hire , press 1 for TATA, 2 for TAVERA, 3 for TOOFAN, 4 for INNOVA \n");
            scanf("%d", &r);
            switch (r)
            {
                case 1:
                printf("\n You have selected TATA SUMO includes fuel cost also | %ldrs per day \n ie total %ldRs\n",20000/nod,20000);
                break;

                case 2:
                printf("\n You have selected TAVERA includes fuel cost also | %ldrs per day \n ie total %ldRs\n",15000/nod,15000);
                break;

                case 3:
                printf("\n You have selected TOOFAN includes fuel cost also | %ldrs per day \n ie total %ldRs\n",12000/nod,12000);
                break;

                case 4:
                printf("\n You have selected INNOVA includes fuel cost also | %1drs per day \n ie total %1drs\n",15500/nod,15500);
                break;

                default:
                printf("You have chosen wrong option\n");
                break;
            }
                printf("Name of the customer : %s \n",name);
    printf("Place of Hiring : %s \n",city);
    printf("Contact number of the Customer is : %s \n",phno);
    printf("Number of days Vehicle is hired : %d \n",nod);
    printf("Registeration number of the hired vehicle : %s \n",vno);
    printf("are you want to confirm the booking\n Yes \n No\n");
    scanf("%s",&cnf);
    compare = strcmp(cnf,"yes");
    if(compare==0){
        break;
    }
    else{
     goto rental;
    }

            case 3:
            printf("\n You have chosen Luxury Cars");
            printf("\n Luxury Vehicles Available are \n");
            printf("\n BENZ, BMW, AUDI \n");
            printf("\n ------------------------------ \n");
            printf("\n Do u want to hire, Press 1 for Benz, 2 for BMW, 3 for Audi \n");
            scanf("%d", &l);

            switch(l)
            {
                case 1:
                printf("\n You have selected Benz includes fuel cost also | Cost %ldrs per day \n ie total %ldRs\n",75000/nod,75000);
                break;

                case 2:
                printf("\n You have selected BMW includes fuel cost also| %ldrs per day \n ie total %ldRs\n",80000/nod,80000);
                break;

                case 3:
                printf("\n You have selected Audi includes fuel cost also| %ldrs per day \n ie total %ldRs\n",50000/nod,50000);
                break;

                default:
                printf("You have chosen wrong option\n");
                break;
            }
    printf("\n ----------------------- \n");
    printf("Name of the customer : %s \n",name);
    printf("Place of Hiring : %s \n",city);
    printf("Contact number of the Customer is : %s \n",phno);
    printf("Number of days Vehicle is hired : %d \n",nod);
    printf("Registeration number of the hired vehicle : %s \n\n",vno);
    printf("are you want to confirm the booking\n Yes \n No\n");
    scanf("%s",&cnf);
    compare = strcmp(cnf,"yes");
    if(compare==0){
        break;
    }
    else{
     goto rental;
    }
            default:
            printf("You have chosen wrong option\n");
            goto rental;
        }
    printf("\n ----------------------- \n");
    printf("\n --------Final Bill-------\n");
    printf("Name of the customer : %s \n",name);
    printf("Place of Hiring : %s \n",city);
    printf("Contact number of the Customer is : %s \n",phno);
    printf("Number of days Vehicle is hired : %d \n",nod);
    printf("Registeration number of the hired vehicle : %s \n",vno);

    return 0;
}
