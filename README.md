package com.example.administrator.actionbarapp;  
  
import android.app.ActionBar;  
import android.app.Activity;  
import android.support.v7.app.ActionBarActivity;  
import android.os.Bundle;  
import android.view.Menu;  
import android.view.MenuItem;  
import android.view.ViewGroup;  
import android.widget.Button;  
import android.widget.CheckBox;  
import android.widget.EditText;  
import android.widget.LinearLayout;  
import android.widget.RadioButton;  
import android.widget.RadioGroup;  
import android.widget.TextView;  
import android.widget.Toast;  
  
  
public class MainActivity extends Activity {  
  
    @Override  
    protected void onCreate(Bundle savedInstanceState) { 
getSupportActionBar().setDisplayHomeAsUpEnabled(false);  
        super.onCreate(savedInstanceState);  
        
  
       
        LinearLayout.LayoutParams params = new LinearLayout.LayoutParams(LinearLayout.LayoutParams.FILL_PARENT, LinearLayout.LayoutParams.WRAP_CONTENT);  
        
        LinearLayout linearLayout = new LinearLayout(this);  
        linearLayout.setOrientation(LinearLayout.VERTICAL);  
  
       
        TextView textView = new TextView(this);  
  
        textView.setText("This TextView is dynamically created");  
        textView.setLayoutParams(params);
       
        EditText editText = new EditText(this);  
        CheckBox checkBox = new CheckBox(this);  
        checkBox.setLayoutParams(params); 
       
        Button button = new Button(this);  
        button.setText("This Button is dynamically created");  
        button.setLayoutParams(params);  
        linearLayout.addView(textView);  
        linearLayout.addView(checkBox);  
        linearLayout.addView(editText);  
        linearLayout.addView(radioGroup);  
        linearLayout.addView(radioButton);  
  
        linearLayout.addView(button);  
 
        LinearLayout.LayoutParams layoutParams = new LinearLayout.LayoutParams(ActionBar.LayoutParams.FILL_PARENT, ActionBar.LayoutParams.WRAP_CONTENT);  
        this.addContentView(linearLayout, layoutParams);  
  
    }  
}

android:layout_width="fill_parent"
android:layout_height="match_parent"
    android:stretchColumns="0,1,2">2"
    android:gravity="center">

    <TableRow
        android:background="#FFFFFF"
        android:layout_width="fill_parent"
        android:layout_height="0dp"
        android:layout_margin="1dp"
        android:layout_weight="1"
        >
        <TableRow
            android:background="#000000"
            android:layout_width="fill_parent"
            android:layout_height="0dp"
            android:layout_margin="1dp"
            android:layout_weight="1"
            >
