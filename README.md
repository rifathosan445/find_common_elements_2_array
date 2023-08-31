# find_common_elements_2_array
Find common elements 2 array and store it 3rd array




    #include<stdio.h>
    int main()
    {
    
      int n1,n2,count=0;
      printf("First Array size= ");
      scanf("%d",&n1);
      int a1[n1],i;
      printf("\n Enter First array elements = ");
      for(i=0;i<n1;i++)
      {
             scanf("%d",&a1[i]);
      }
    
      printf("2nd array size = ");
      scanf("%d",&n2);
      int a2[n2],j;
      printf("\n Enter 2nd array elements = ");
      for(j=0;j<n2;j++)
      {
             scanf("%d",&a2[j]);
      }
      int a3[count],k=0;
      if(i<j)
      {
         for(i=0;i<n1;i++)
         {
                for(j=0;j<n2;j++)
                {
                       if(a1[i]==a2[j])
                       {
                          a3[k] = a1[i] ;
                          k++;
                          count++;
                          break;
    
                       }
    
                }
         }
          printf("\n\nCommon Element array= ");
         for(k=0;k<count;k++)
         {
             printf("%d,",a3[k]);
    
         }
      }
    
      return 0;
    }
    
