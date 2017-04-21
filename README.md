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


struts.xml
<!DOCTYPE struts PUBLIC
    "-//Apache Software Foundation//DTD Struts Configuration 2.0//EN"
    "http://struts.apache.org/dtds/struts-2.0.dtd">

To avoid request from being null:

request = new MockHttpServletRequest();
For session:

Map<String, Object> sessionMap = new HashMap<String, Object>();
actionProxy.getInvocation().getInvocationContext().setSession(sessionMap);

In my case I needed to call super.setUp from my test.


@Before
31     public void setUp() throws Exception {
32         //這幾行一定要寫
33             //等價於在 web.xml 中設定 <init-param> 參數
34         Map<String, String> dispatcherInitParams = new HashMap<String, String>();
35         ReflectionTestUtils.setField(this, "dispatcherInitParams", dispatcherInitParams);
36             //載入 struts 設定檔
37         dispatcherInitParams.put("config", "struts-default.xml,struts-plugin.xml,struts.xml");
38         
39         super.setUp();
40     }

initServletMockObjects();

com.opensymphony.xwork2.config.ConfigurationException: Unable to load configuration
