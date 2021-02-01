int[] findTwoElement(int arr[], int n) {
        // code here
        int repeat, miss;
        int s=n*(n+1)/2;
        int s2 = n*(n+1)*(2*n+1)/6;
        int dif=s;
        for(int x : arr)
            dif-=x;
        int dif2=s2;
        for(int x : arr){
            dif2-=x*x;
        }
        int sum = dif2/dif;
        miss=(sum+dif)/2;
        repeat=sum-miss;
        return new int[] {repeat, miss};
    }
 <---------------------------or--------------------------->
    int[] findTwoElement(int arr[], int n) {
        // code here
        int[] ans = new int[2];
        int i;
        for (i = 0; i < n; i++) {
            int abs_val = Math.abs(arr[i]);
            if (arr[abs_val - 1] > 0)
                arr[abs_val - 1] = -arr[abs_val - 1];
            else
                ans[0] = abs_val;
        }
        for (i = 0; i < n; i++) {
            if (arr[i] > 0) ans[1] = i + 1;
        }
        return ans;
    }
