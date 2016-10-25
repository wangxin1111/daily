#2016年10月19日
====================
 1.已完成内容
•	Android studio 布局
 	

2.工作成果


package com.example.administrator.myapplication;

import android.app.Activity;
import android.graphics.Color;
import android.os.Bundle;
import android.view.ViewGroup;
import android.widget.Button;
import android.widget.LinearLayout;
import android.widget.RelativeLayout;
import android.widget.TextView;

public  class MainActivity extends Activity {
@SuppressWarnings("ResourceType")
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);

    LinearLayout linearLayoutAll = new LinearLayout(this);
    linearLayoutAll.setOrientation(LinearLayout.VERTICAL);

    // 定义线性布局1
    TextView textView =new TextView(this);
    textView.setHeight(1100);
    textView.setBackgroundColor(Color.CYAN);

    LinearLayout linearLayout = new LinearLayout(this);
    linearLayout.setOrientation(LinearLayout.HORIZONTAL);

    Button button1 = new Button(this);
    button1.setText("按钮1");
    Button button2 = new Button(this);
    button2.setText("按钮2");
    Button button3 = new Button(this);
    button3.setText("按钮3");
    Button button4 = new Button(this);
    button4.setText("按钮4");
    linearLayout.addView(button1);
    linearLayout.addView(button2);
    linearLayout.addView(button3);
    linearLayout.addView(button4);
// 定义线性布局 2
    LinearLayout linearLayout1 = new LinearLayout(this);
    linearLayout1.setOrientation(LinearLayout.HORIZONTAL);
    Button button5 = new Button(this);
    button5.setText("按钮5");
    Button button6 = new Button(this);
    button6.setText("按钮6");
    Button button7 = new Button(this);
    button7.setText("按钮7");
    Button button8 = new Button(this);
    button8.setText("按钮8");
    linearLayout1.addView(button5);
    linearLayout1.addView(button6);
    linearLayout1.addView(button7);
    linearLayout1.addView(button8);

    // 定义线性布局 3

    LinearLayout linearLayout2 = new LinearLayout(this);
    linearLayout2.setOrientation(LinearLayout.HORIZONTAL);
    Button button9 = new Button(this);
    button9.setText("按钮9");
    Button button10 = new Button(this);
    button10.setText("按钮10");
    Button button11 = new Button(this);
    button11.setText("按钮11");
    Button button12 = new Button(this);
    button12.setText("按钮12");
    linearLayout2.addView(button9);
    linearLayout2.addView(button10);
    linearLayout2.addView(button11);
    linearLayout2.addView(button12);

    // 定义线性布局 4

    LinearLayout linearLayout3 = new LinearLayout(this);
    linearLayout3.setOrientation(LinearLayout.HORIZONTAL);
    Button button13 = new Button(this);
    button13.setText("按钮13");
    Button button14 = new Button(this);
    button14.setText("按钮14");
    Button button15 = new Button(this);
    button15.setText("按钮15");
    Button button16 = new Button(this);
    button16.setText("按钮16");
    linearLayout3.addView(button13);
    linearLayout3.addView(button14);
    linearLayout3.addView(button15);
    linearLayout3.addView(button16);





    //
    linearLayoutAll.addView(textView);
    linearLayoutAll.addView(linearLayout);
    linearLayoutAll.addView(linearLayout1);
    linearLayoutAll.addView(linearLayout2);
    linearLayoutAll.addView(linearLayout3);

    setContentView(linearLayoutAll);




3.未完成工作**
 


4.未完成原因
 

5.遇到的问题及解决方案
 


