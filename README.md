
My ViewInject
========

### Example


#### First Init
```java
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        //setContentView(R.layout.activity_retrofit);
        ViewUtils.register(this);
    }
```

#### Second
```java
   @ViewLayout(R.layout.activity_retrofit)
   public class Activity{
```

#### Third
```java
    @ViewMethod(getId = R.id.activity_retrofit_test1)
    private void test1(View view){
        //do something
    }

    @ViewField(getId = R.id.activity_retrofit_title)
    TextView title;
```
