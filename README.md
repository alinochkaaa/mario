# include <stdio.h>
# include <cs50.h>

int main(void)
{
    int height;
    do
    {
        printf ("Write the height of pyramid. Height must be not less than 0 and not greater than 23!\n");
        height = GetInt();
    }
    while ((height<0) || (height>23));
    {
        for (int x=2; x<height+2; x++)
        {
            for (int s=height+1; s>x; s--)
            { 
                printf (" ");
            }
            for (int d=2; d<x+2; d++)
            {
                printf ("#");
            }  
        printf ("\n");
        }
    }
}
