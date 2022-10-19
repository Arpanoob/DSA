class Solution
{
    //Function to return the total number of possible unique BST.
    static long dp[];
    static long solve(int N){
        if(N==1 || N==0) return 1;
        if(N==2) return 2;
        if(dp[N]!=0) return dp[N];
        for(int i=0;i<N;i++){
            dp[N]=(dp[N]+(solve(i)*solve(N-i-1))%1000000007)%1000000007;
        }
        return dp[N];
    }
    static int numTrees(int N)
    {
        // Your code goes here
        dp=new long[N+1];
        return (int)(solve(N)%1000000007);
    }
}
