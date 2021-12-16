# TinyDB

public class MainActivity extends AppCompatActivity {
    TinyDBSharedPref tinyDBSharedPref = null;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_home_screen);

        tinyDBSharedPref=new TinyDBSharedPref(MainActivity.this);
        
        //To Save Value in TinyDb
        //For String Value
          --->Save
          tinyDBSharedPref.putString("value","Saved Value");
          --->Get
           tinyDBSharedPref.getString("value");

   
    }
}
