# error-
    The type android.support.v4.app.TaskStackBuilder$SupportParentable cannot be resolved. It is indirectly referenced from required 
.class files错误的解决

    今天在使用v7的的ActionBar，在继承ActionBarActivity时报了The type Android.support.v4.app.TaskStackBuilder$SupportParentable 
cannot be resolved. It is indirectly referenced from required .class files”错误，网上查了很久解决了。

    问题根源：因为在复制项目的jar包时，把Eclipse下自带的android-support-v4.jar包复制到了‘android-support-v7-appcompat’ Library项目下，
替换掉了原本的android-support-v4.jar，而Eclipse自带的版本较低，导致报错。

    解决方案：当然把android-support-v4.jar替换成..\sdk\extras\android\support\v7\appcompat\libs下的android-support-v4.jar的啦。
