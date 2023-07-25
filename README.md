# c---problrm-solving

program to remove space


#include <stdio.h>
#include <string.h>

int main()
{
    char a[100];
    scanf("%[^\n]s",a);
    
    for(int i=0;i<strlen(a);i++)
    {
        if(a[i]==' ')
        continue;
        else
        printf("%c",a[i]);
    }
      
    return 0;
}



2. sort string in alphabatical order
3. 
#include <stdio.h>
#include <string.h>

int main()
{
    char a[100];
    scanf("%s",a);
    
    for(int i=0;i<strlen(a);i++){
        for(int j=i+1;j<strlen(a);j++)
        {
            if(a[i]>a[j])
            {
                char t=a[i];
                a[i]=a[j];
                a[j]=t;
            }
        }
        printf("%C",a[i]);
    }
    
}
