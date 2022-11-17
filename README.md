//# BoB_solve_2
#include<stdio.h>
int main()
{
    int t;
    scanf("%d",&t);
    while(t--)
    {
        int n,s=0,p,q,e=0;
        scanf("%d",&n);
        int arr[100];
        for(int i=0;i<n;i++)
        {
            scanf("%d",&arr[i]);
        }
        for(int j=0;j<n;j++)
        {
            s+=arr[j];
        }
        for(int k=0;k<n;k++)
        {
            p=s-arr[k];
            q=p+(-(arr[k]));
            if(q%2==0)
            {
                e++;
            }
        }
        printf("%d\n",e);
    }
    return 0;
}
