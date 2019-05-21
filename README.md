# android-Display-width-height
get your device display width &amp; height any where

1-create Class Common.java
    
    public class Common {
    public static int displayWidth(Context context) {
    WindowManager wm = (WindowManager) context.getSystemService(Context.WINDOW_SERVICE);
    Display display = wm.getDefaultDisplay();
    Point size = new Point();
    display.getSize(size);
    return size.x;
    }

    public static int displayHeight(Context context) {
    WindowManager wm = (WindowManager) context.getSystemService(Context.WINDOW_SERVICE);
    Display display = wm.getDefaultDisplay();
    Point size = new Point();
    display.getSize(size);
    return size.y;
    }
    }
    
2-use this any where:

    int with = displayWidth(activity);
    int height = displayHeight(activity);


