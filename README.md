# array-basic-operations-like-add-and-multiply
# I just tried to perform addition and multiplication for 2d array
import java.util.Scanner;
class Main {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int[][] a = new int[3][3];
        int[][] b = new int[3][3];
        int[][] c = new int[3][3]; 
        int[][] d = new int[3][3]; 
        for(int q=0;q<a.length;q++)
        {
           for(int w=0;w<a.length;w++)
           {
               System.out.print("enter a["+q+"]["+w+"]:");
               a[q][w]=sc.nextInt();
           }
        }
        for(int i=0;i<a.length;i++)
        {
            for(int j=0;j<a[i].length;j++)
            {
              System.out.print(a[i][j]+" ");
            }
            System.out.println(" ");
    }
         for(int e=0;e<a.length;e++)
        {
           for(int r=0;r<a.length;r++)
           {
               System.out.print("enter b["+e+"]["+r+"]:");
               b[e][r]=sc.nextInt();
           }
        }
        for(int m=0;m<a.length;m++)
        {
            for(int g=0;g<a[m].length;g++)
            {
              System.out.print(b[m][g]+" ");
            }
            System.out.println(" ");
       }
       for(int z=0;z<a.length;z++)
       {
           for(int x=0;x<a[z].length;x++)
           {
               c[z][x]=a[z][x]+b[z][x];
           }
       }
       for(int V=0;V<c.length;V++)
        {
           for(int B=0;B<c.length;B++)
           {
               System.out.print(c[V][B]+" ");
           }
           System.out.println(" ");
        }
       for(int h=0;h<a.length;h++)
        {
           for(int n=0;n<b[h].length;n++)
           {
               for(int y=0;y<b.length;y++)
               {
                  d[h][n]+=a[h][y]*b[y][n];
               }}}
               
          for(int p=0;p<d.length;p++)
        {
           for(int s=0;s<c.length;s++)
           {
               System.out.print(d[p][s]+" ");
           }
           System.out.println(" ");
        }
    }
}
