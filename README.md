# Ex_No-9_Graphical-Primitives
Design an application that draws basic graphical primitives on the screen.

## AIM:
To create and design an android application that draws basic graphical primitives on the screen using Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)


## ALGORITHM:
Step 1: Open Android Studio and then click on File -> New -> New project.

Step 2: Then type the Application name as SMSIntent and click Next.

Step 3: Select the Minimum SDK below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally, click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Draw the basic object processed in MainActivity file.

Step 7: Save and run the application.


## Program:
 ```
/*
Program to create and design an android application for draw basic graphical primitives.
Developed by:LOGESHWARI.P 
RegisterNumber:212221230055  
*/
```

## MainActivity.java:
```
package com.example.ex_10;

import android.graphics.Bitmap;
import android.graphics.Canvas;
import android.graphics.Color;
import android.graphics.Paint;
import android.graphics.drawable.BitmapDrawable;
import android.os.Bundle;
import android.widget.ImageView;

import androidx.appcompat.app.AppCompatActivity;
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Bitmap bg = Bitmap.createBitmap(720, 1280,
                Bitmap.Config.ARGB_8888);
        ImageView i = (ImageView) findViewById(R.id.ImageView);
        i.setBackgroundDrawable(new BitmapDrawable(bg));
        Canvas canvas = new Canvas(bg);
        Paint paint = new Paint();
        Paint paint1 = new Paint();
        Paint paint2 = new Paint();
        Paint paint3 = new Paint();
        Paint paint4 = new Paint();
        paint.setColor(Color.RED);
        paint1.setColor(Color.BLUE);
        paint2.setColor(Color.MAGENTA);
        paint3.setColor(Color.GREEN);
        paint4.setColor(Color.BLACK);
        paint.setTextSize(50);
        paint1.setTextSize(50);
        paint2.setTextSize(50);
        paint3.setTextSize(50);
        paint4.setTextSize(50);
        canvas.drawText("Rectangle", 420, 150, paint4);
        canvas.drawRect(400, 200, 650, 700, paint);
        canvas.drawText("Circle", 120, 150, paint4);
        canvas.drawCircle(200, 350, 150, paint1);
        canvas.drawText("Square", 120, 800, paint4);
        canvas.drawRect(50, 850, 350, 1150, paint2);
        canvas.drawText("Line", 480, 800, paint4);
        canvas.drawLine(520, 850, 520, 1150, paint3);

    }
}
```
## activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout android:layout_height="match_parent"
    android:layout_width="match_parent"
    xmlns:android="http://schemas.android.com/apk/res/android">
    <ImageView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:id="@+id/ImageView"/>
</RelativeLayout>
```
## Output:
![244914581-a2cb1eb4-d8f0-4232-9608-6218906795b9](https://github.com/logeshwari2004/Ex_No-9_Graphical-Primitives/assets/94211349/5f806b72-7368-4f65-8504-0efadc1f5563)



## Result:
Thus a Simple Android Application to create and design an android application that draws basic graphical primitives on the screen using Android Studio was developed and executed successfully.
