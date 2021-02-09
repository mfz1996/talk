**发送给璐璐的消息存在这里**
    private int test(int[][] nums,int x, int y){
        int width = Math.max(Math.abs(x),Math.abs(y))*2+1;
        int maxVal = width*width;
        int result;
        if (x>=0 && y>=0){
            result = maxVal-3*(width-1)-x+y;
        }else if (x<= 0&& y>=0){
            result = maxVal-2*(width-1)-x-y;
        }else if (x<= 0&& y<0){
            result = maxVal-2*(width-1)+x-y;
        }else{
            result = maxVal-2*(width-1)+x+y;
        }
        return result;
    }
