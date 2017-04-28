SDK Tools Release Notes: https://developer.android.com/studio/releases/sdk-tools.html
SDK Platform Tools Release Notes: https://developer.android.com/studio/releases/platforms.html

To download a manual version of SDK Tools, fill in the following url with a version from the above:

https://dl-ssl.google.com/android/repository/tools_r<version>-windows.zip
https://dl-ssl.google.com/android/repository/tools_r<version>-macosx.zip

For me downgrading to https://dl-ssl.google.com/android/repository/tools_r25.2.5-macosx.zip worked just fine. Once you download an older version the tools, just rename the tools directory at your Android SDK install and replace with the downloaded version.

I didn't need to downgrade Platform Tools, but if you need to, here are those links as well:

https://dl-ssl.google.com/android/repository/platform-tools_r<version>-windows.zip
https://dl-ssl.google.com/android/repository/platform-tools_r<version>-macosx.zip



Arquillian, a powerful container-oriented testing framework layered atop TestNG and JUnit, gives you the ability to create the production environment on the container of your choice and just execute tests in that environment (using the datasources, JMS destinations, and a whole lot of other configurations you expect to see in production environment). Instead of bringing your runtime to the test, Arquillian brings your test to the runtime




Error creating bean with name 'scopedTarget.sysUser': Scope 'session' is not active for the current thread; consider defining a scoped proxy for this bean if you intend to refer to it from a singleton


[testng] An error occurred while instantiating class org/apache/logging/log4j/LogManager

java.lang.StackOverflowError
	at org.apache.logging.log4j.spi.LoggerRegistry.getOrCreateInnerMap(LoggerRegistry.java:140)
java.lang.NoClassDefFoundError: javax/servlet/jsp/PageContext

javax.servlet:servlet-api and javax.servlet.jsp:jsp-api
