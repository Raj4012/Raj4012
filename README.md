- 👋 Hi, I’m @Raj4012
- 👀 I’m interested in full stack develpoment and Machine learning.
- 🌱 I’m currently learning full stack develoment
- 💞️ I’m looking to collaborate on any new full stack dev projects
- 📫 How to reach me kumarrajbharti278290@gmail.com
- 😄 Pronouns: Raj_4_04
- ⚡ Fun fact: ...

<!---
Raj4012/Raj4012 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


class Solution {
    public  static int findTheDistanceValue(int[] arr1, int[] arr2, int d) {
        int count = 0;

        for(int num1 : arr1){
            boolean isValid = true;
            for(int num2 : arr2){
                if(Math.abs(num1 - num2) <= d){
                    isValid = false;
                    break;
                }
            }
            if (isValid){
                count++;
            }
        }
        return count;
    }
    public static void main(String args[]){
        int[] arr1 = {4,5,8};
        int [] arr2 = {10,9,1,8};
        int d = 2;

        System.out.println(findTheDistanceValue(arr1, arr2, d));

        arr1 = new int[]{1,4,2,3};
        arr2 = new int[]{-4,-3,6,10,20,30};
        d = 3;

        System.out.println(findTheDistanceValue(arr1, arr2, d));

        arr1 = new int[]{2,1,100,3};
        arr2 = new int[]{-5,-2,10,-3,7};
        d = 6;
        System.out.println(findTheDistanceValue(arr1, arr2, d));
    }  
}
