19 public class ScenarioHook extends Base{
20 
21     //RemoteWebDriver remoteDriver;
22     WebDriver driver;
23     @Before
24     public void setup()
25     {
26 
27         try {
28             String browser=this.getBrowser();
29 
30             //System.out.println("java -jar src/main/resources/selenium-server-4.41.0.jar
31             if (browser.equals("chrome")) {
32                 driver = new ChromeDriver();
33                 //System.out.println("***REACHED IF");
34                 /* ChromeOptions options = new ChromeOptions();
35                 options.setCapability("platformName", "Windows");
36 
37                 remoteDriver = new RemoteWebDriver(
38                     new URL("http://localhost:4444"),options
39 
40                 );*/
41 
