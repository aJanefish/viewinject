
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



Download
--------
### How to
Step 1. Add the JitPack repository to your build file
Add it in your root build.gradle at the end of repositories:

```groovy
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
```

Step 2. Add the dependency

```groovy
implementation 'com.github.aJanefish:viewinject:Tag'
```




