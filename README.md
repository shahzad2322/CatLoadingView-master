# Android LoadingView MAster BESt 

This project idea is from [Link](http://mp.weixin.qq.com/s?__biz=MjM5MDMxOTE5NA==&mid=402703079&idx=2&sn=2fcc6746a866dcc003c68ead9b68e595&scene=2&srcid=0302A7p723KK8E5gSzLKb2ZL&from=timeline&isappinstalled=0#wechat_redirect).<br>
Thanks for the idea.<br>

I like the animation in this picture:<br>


...as you see it right now, I hope you like it!

### Step

Import this project into Android Studio... it's built with it.

###  Usage

#### Gradle

```
implementation 'com.github.shahzad2322:CatLoadingView-master:1.0'
```

####  config in java code

    CatLoadingView mView;


    @Override protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        
        mView = new CatLoadingView();
        findViewById(R.id.button).setOnClickListener(
                new View.OnClickListener() {
                    @Override public void onClick(View v) {
                        mView.show(getSupportFragmentManager(), "");
                    }
                });
    }

## TODO

This view is adjusted in Nexus5 but not tested on other screen sizes.



