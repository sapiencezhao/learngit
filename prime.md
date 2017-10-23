void printPrime(int n){//判断n是否是质数
        boolean isPrime=true;//是否是质数的标志
        for(int i=n-1;i>1;i—){//n除以每个比n小比1大的自然数
            if(n%i==0){//如果有能被整除的，则不是质数
                isPrime=false;
            }
        }
        if(isPrime){//如果是质数，则打印出来
            System.out.print(n+" ");
            primeNumber++;//记录质数的个数
            if(primeNumber%10==0)//输出10个质数后换行
                System.out.println();
        }
}