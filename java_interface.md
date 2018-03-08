```java

class MyCalculator implements AdvancedArithmetic {
        public int divisor_sum(int n) {
//         create placeholder arrayList of divisors
            LinkedList<Integer> divisors = new LinkedList<Integer>();

                // System.out.println(divisors);

//          loop until reaching n max value of 12
            for(int i = 1; i <= n; i++) {

//         if divisible by current element at index then add to divisors
                // System.out.println(i);
                if (n%i == 0) {
                    // System.out.println(i);
                    divisors.add(i);
                }
            }

                // System.out.println(divisors);
//         use reduce method to find sum of divisors arrayList
            int sum = 0;
            for(int divisor: divisors) {
                sum += divisor;
            }

            // System.out.println(sum);
        return sum;
    }
}
```