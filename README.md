# ionic_issue_6260_reproduction
reproduction of issue https://github.com/ionic-team/capacitor/issues/6260

steps to reproduce:

1. go to `./myTestApp/android`
2. run `./gradlew lint`

output:

<pre><code>
myTestApp/node_modules/@capacitor/android/capacitor/src/main/java/com/getcapacitor/Bridge.java:324: Error: Unnecessary; SDK_INT is always >= 30 [ObsoleteSdkInt]
        if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.O) {
            ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
</code></pre>
