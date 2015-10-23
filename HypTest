#include <stdio.h>
#include <stdlib.h>

int main()
{
    intN,DOF,i,n;
    intX=0,Y=0,x=0,y=0,sumx=0,sumy=0,sumsqx=0,sumsqy=0,meanX=0,meanY=0,sxtl=0,
sxsqrt=0,sytl=0,sysqrt=0,xy=0,xx=0,yy=0,sxx=0,syy=0;
    double LOS,c;
    double sx=0,sy=0,nmeanxy=0,R=0,T=0;

    FILE*ip_file;

    ip_file = fopen("input1.txt", "r");
    if (ip_file == NULL)
        {
            printf("input file could not be opened\n");
            exit(1);
         }

    //Retrieves values from the file and calculates the sum.
    fscanf(ip_file, "%d",&N);


    printf("Please enter an appropriate Level of Significance:\n");
    scanf("%lf",&LOS);
    printf("\n\nThe Null Hypothesis is that there is no correlation.\n\nThe Alternative Hypothesis is that there is correlation");
    printf("\n\nThe LOS is:%.3lf",LOS);
    printf("\n\nDegrees of Freedom = %d",N-2);

    for (i=0;i<N;i++){
    fscanf(ip_file, "%d",&x);
    sumx+=x;
    }

   for (i=0;i<N;i++){
    fscanf(ip_file, "%d",&y);
    sumy+=y;
    }

   fclose(ip_file);

//opening file to use the values for x and y to get the sum(squared)

  FILE*i_file;

    i_file = fopen("input1.txt", "r");
    if (i_file == NULL)
        {
            printf("input file could not be opened\n");
            exit(1);
         }

   fscanf(i_file, "%d",&n);

    for (i=0;i<n;i++){
    fscanf(i_file, "%d",&X);
    sumsqx+=X*X;
    }

    for (i=0;i<n;i++){
    fscanf(i_file, "%d",&Y);
    sumsqy+=Y*Y;
    }

    //Calculates the mean of X and Y.
    meanX=sumx/N;
    meanY=sumy/N;
    
    //Calculation of the standard deviation
    sxtl = sumsqx-n*(meanX*meanX);
    sxsqrt=sxtl/(N-1);
    sx=sqrt(sxsqrt);

    sytl = sumsqy-n*(meanY*meanY);
    sysqrt=sytl/(N-1);
    sy=sqrt(sysqrt);

//Calculation of values required for R calculation
    xy=sumx*sumy;
    nmeanxy=N*sx*sy;
    xx=sumsqx-N*sx*sx;
    sxx=sqrt(xx);
    yy=sumsqy-N*sy*sy;
    syy=sqrt(yy);
    
//Calculate R
    R=(xy-nmeanxy)/(sxx*syy);
//Calculate T

    T=R*sqrt(N-2/(1-(R*R)));

    printf("\n\n\t****Data****\n");
    printf("N = %d",N);
    printf("\nThe sum of X = %d",sumx);
    printf("\nThe sum of Y = %d",sumy);
    printf("\nThe sum squared of X = %d",sumsqx);
    printf("\nThe sum squared of Y = %d",sumsqy);
    printf("\nThe mean of X = %d",meanX);
    printf("\nThe mean of Y = %d",meanY);
    printf("\nThe standard deviation of X = %lf",sx);
    printf("\nThe standard deviation of Y = %lf",sy);
    printf("\nR=%lf",R);
    printf("\nT=%lf",T);

// To get the critical value
     if(LOS=0.05){
          if (DOF=1){
            c = 6.314;
          };
            if (DOF=2){
                c=2.920;
            };
            if (DOF=3){
                c=2.353;
            };
            if (DOF=4){
                c=2.132;
            };
            if(DOF=5){
                c=2.015;
            };
            if(DOF=6){
                c=1.943;
            };
            if(DOF=7){
                c=1.895;
            };
            if(DOF=8){
                c=1.860;
            };
            if(DOF=9){
                c=1.833;
            };
            if(DOF=10){
                c=1.812;
            };
            if(DOF=11){
                c=1.796;
            };
            if(DOF=12){
                c=1.782;
            };
            if(DOF=13){
                c=1.771;
            };
            if(DOF=14){
                c=1.761;
            };
            if(DOF=15){
                c=1.753;
            };
            if(DOF=16){
                c=1.746;
            };
            if(DOF=17){
                c=1.740;
            };
            if(DOF=18){
                c=1.734;
            };
            if(DOF=19){
                c=1.729;
            };
            if(DOF=20){
                c=1.725;
            };
            if(DOF=21){
                c=1.721;
            };
            if(DOF=22){
                c=1.717;

            };
            if(DOF=23){
                c=1.714;

            };
             if(DOF=24){
                c=1.711;

            };
             if(DOF=25){
                c=1.708;

            };
             if(DOF=26){
                c=1.706;

            };
          };
         if (LOS=0.025){
          if (DOF=1){
            c=12.706;
          };
            if (DOF=2){
                c=4.303;
            };
            if (DOF=3){
                c=3.182;
            };
            if (DOF=4){
                c=2.776;
            };
            if(DOF=5){
                c=2.571;
            };
            if(DOF=6){
                c=2.447;
            };
            if(DOF=7){
                c=2.365;
            };
            if(DOF=8){
                c=2.306;
            };
            if(DOF=9){
                c=2.262;
            };
            if(DOF=10){
                c=2.228;
            };
            if(DOF=11){
                c=2.201;
            };
            if(DOF=12){
                c=2.179;
            };
            if(DOF=13){
                c=2.160;
            };
            if(DOF=14){
                c=2.145;
            };
            if(DOF=15){
                c=2.131;
            };
            if(DOF=16){
                c=2.120;
            };
            if(DOF=17){
                c=2.110;
            };
            if(DOF=18){
                c=2.101;
            };
            if(DOF=19){
                c=2.093;
            };
            if(DOF=20){
                c=2.086;
            };
            if(DOF=21){
                c=2.080;
            };
            if(DOF=22){
                c=2.074;

            };
            if(DOF=23){
                c=2.069;

            };
             if(DOF=24){
                c=2.064;

            };
             if(DOF=25){
                c=2.060;

            };
             if(DOF=26){
                c=2.056;

            };
          };

         if (LOS=0.01){
          if (DOF=1){
            c=31.821;
          };
            if (DOF=2){
                c=6.965;
            };
            if (DOF=3){
                c=4.541;
            };
            if (DOF=4){
                c=3.747;
            };
            if(DOF=5){
                c=3.365;
            };
            if(DOF=6){
                c=3.143;
            };
            if(DOF=7){
                c=2.998;
            };
            if(DOF=8){
                c=2.896;
            };
            if(DOF=9){
                c=2.821;
            };
            if(DOF=10){
                c=2.764;
            };
            if(DOF=11){
                c=2.718;
            };
            if(DOF=12){
                c=2.681;
            };
            if(DOF=13){
                c=2.650;
            };
            if(DOF=14){
                c=2.624;
            };
            if(DOF=15){
                c=2.602;
            };
            if(DOF=16){
                c=2.583;
            };
            if(DOF=17){
                c=2.567;
            };
            if(DOF=18){
                c=2.552;
            };
            if(DOF=19){
                c=2.539;
            };
            if(DOF=20){
                c=2.528;
            };
            if(DOF=21){
                c=2.518;
            };
            if(DOF=22){
                c=2.508;

            };
            if(DOF=23){
                c=2.500;

            };
             if(DOF=24){
                c=2.492;

            };
             if(DOF=25){
                c=2.485;

            };
             if(DOF=26){
                c=2.479;

            };
          };


          if(LOS=0.005){
          if (DOF=1){
            c=63.657;
          };
            if (DOF=2){
                c=9.925;
            };
            if (DOF=3){
                c=5.841;
            };
            if (DOF=4){
                c=4.604;
            };
            if(DOF=5){
                c=4.032;
            };
            if(DOF=6){
                c=3.707;
            };
            if(DOF=7){
                c=3.499;
            };
            if(DOF=8){
                c=3.355;
            };
            if(DOF=9){
                c=3.250;
            };
            if(DOF=10){
                c=3.169;
            };
            if(DOF=11){
                c=3.106;
            };
            if(DOF=12){
                c=3.055;
            };
            if(DOF=13){
                c=3.012;
            };
            if(DOF=14){
                c=2.977;
            };
            if(DOF=15){
                c=2.947;
            };
            if(DOF=16){
                c=2.921;
            };
            if(DOF=17){
                c=2.898;
            };
            if(DOF=18){
                c=2.878;
            };
            if(DOF=19){
                c=2.861;
            };
            if(DOF=20){
                c=2.845;
            };
            if(DOF=21){
                c=2.831;
            };
            if(DOF=22){
                c=2.819;

            };
            if(DOF=23){
                c=2.807;

            };
             if(DOF=24){
                c=2.797;

            };
             if(DOF=25){
                c=2.787;

            };
             if(DOF=26){
                c=2.229;

            };
          };



 printf("\n\nThe Critical Value is = %.3lf",c);

   if (T<c){
    printf("\n\n\nThe Null Hypothesis is rejected as the Critical value is less than \nthe Calculated value\n\n");
    };

    if(T>c){
        printf("\n\n\nThe Null Hypothesis is accepted as our calculated value for\nT is larger than our critical value \n\n");
    };


 fclose(ip_file);
    return 0;
}
