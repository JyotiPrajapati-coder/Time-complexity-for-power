# Time-complexity-for-power
Help me to reduce its time complexity
class Solution {
public:
    double myPow(double x, int n) {
        double power=1;
        if(n>0){
            for(int i=0;i<n;i++){
                power=power*x;
            }
        }
        else if(n<0){
            double j=1/x;
            for(int i=0;i<-(n);i++){
                power=power*j;
            }
            
        }
        else{
            power=1;
        }
        return power;
    }
};    