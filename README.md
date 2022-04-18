# using_SHAFT_ENGINE

<img src="https://github.com/MohabMohie/SHAFT_ENGINE/raw/master/src/main/resources/images/shaft.png" alt="SHAFT_ENGINE" style="display:block; margin-left:auto; margin-right:auto;"/>

**using_SHAFT_ENGINE** is a sample project to showcase how to get started using [SHAFT_Engine](https://github.com/MohabMohie/SHAFT_ENGINE/), and how to use some of its rich features, while applying the best practices for Test Automation project design. For a full list of the Supported features that you can use or try out, please refer to this [Read Me](https://github.com/MohabMohie/SHAFT_ENGINE/blob/master/README.md) file.

### Running your first sample test:

1. Simply import this project to your eclipse (or favorite JAVA IDE).
2. Watch this simple 5-minute live-demo:
   https://drive.google.com/file/d/1NxBpObvbBHdMjL4tl7PlpRNi7U9lMfW8/view

### Creating your own project based on using_SHAFT_ENGINE:

1. Make your own fork from the project <img src="https://drive.google.com/uc?export=download&id=1TIHfU4OamNjqEHFhasxw6tUw8YJwrItX" alt="using_SHAFT_ENGINE" style="display:block; margin-left:auto; margin-right:auto;"/>
2. Check out the Maven Projects from Git (File - Import - Maven -Check out Maven Projects from SCM)
   2.1. On the window that is presented click the link "Find more SCM connectors in the m2e Marketplace" in the bottom right corner of the page.
   2.2. Search for "m2e-egit" and install it, then restart and continue.
3. After your project is successfully imported, you can explore the file structure, and add your own tests or test suites as needed.

### Important Notes:

-   Always use the latest version of SHAFT_Engine in your pom.xml file

    ![Bintray](https://img.shields.io/bintray/dt/mohabmohie/SHAFT/SHAFT_Engine?color=blue&label=Total%20Downloads&style=for-the-badge)
    [![Bintray](https://img.shields.io/bintray/v/mohabmohie/SHAFT/SHAFT_Engine?label=Bintray&style=for-the-badge)](https://bintray.com/mohabmohie/SHAFT/SHAFT_Engine/_latestVersion)
    [![Maven Central](https://img.shields.io/maven-central/v/io.github.mohabmohie/SHAFT_ENGINE?style=for-the-badge)](https://search.maven.org/search?q=g:%22io.github.mohabmohie%22%20AND%20a:%22SHAFT_ENGINE%22)

-   Refer to the published SHAFT_Engine javadocs for detailed information on the available functions/classes/packages https://mohabmohie.github.io/SHAFT_ENGINE/
-   Refer to TestNG [https://testng.org/doc/documentation-main.html] and Allure Reporting [https://docs.qameta.io/allure/] documentation for using annotations
-   Refer to the latest Sample Test Execution report for more info [https://mohabmohie.github.io/using_SHAFT_ENGINE/allure]

### IntelliJ:

-   As of SHAFT_Engine '4.0.20200220-beta' you can now use IntelliJ in addition to Eclipse to manage your test project.
-   After checking out the project to your IntelliJ you may face an exception that prevents tests execution.
-   In that case you need to add the SHAFT_Engine custom listeners to your TestNG execution template, as IntelliJ doesn't natively inherit this list from the pom.xml file.
-   Here are the steps you need to follow:


    -   This is the error that you may see <img src="readMeImgs/1.PNG" alt="1 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>
    -   In that case you need to Edit your Run/Debug configuration <img src="readMeImgs/2.PNG" alt="2 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>
    -   Delete the existing configurations <img src="readMeImgs/3.png" alt="3 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>

    -   Click on Edit configuration template <img src="readMeImgs/4.png" alt="4 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>

    -   Navigate to TestNG > Configuration > Listeners <img src="readMeImgs/5.PNG" alt="5 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>
    -   Type com.shaft.tools.\* into your search box to find the required listeners and add them one by one <img src="readMeImgs/5.png" alt="5 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>
    -   This is the desired output for your listeners configuration <img src="readMeImgs/6.PNG" alt="6 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>
    -   Success! <img src="readMeImgs/7.PNG" alt="7 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>
    -   Click on Edit configuration template <img src="https://drive.google.com/uc?export=download&id=1wwBFObeWE6Nr-yo2t8qUNWbL5VeSdOJJ" alt="4 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>

    -   Navigate to TestNG > Configuration > Listeners <img src="https://drive.google.com/uc?export=download&id=1-WqbA2EPvMXX55Dr7pnQLUtnZ4OWwfAN" alt="5 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>
    -   Type com.shaft.tools.\* into your search box to find the required listeners and add them one by one <img src="https://drive.google.com/uc?export=download&id=17lykJyCaCTYgnmZY0NBzfWxWLQGzxOyU" alt="4 of 6" style="display:block; margin-left:auto; margin-right:auto;"/>
    -   This is the desired output for your listeners configuration <img src="https://drive.google.com/uc?export=download&id=1h047bFULAzItLr2yJ_LNnIToJjRttUDX" alt="6 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>
    -   Success! <img src="https://drive.google.com/uc?export=download&id=1TiFuFW2s2hozOtkM9t-ZBWbOEdQssV6g" alt="7 of 7" style="display:block; margin-left:auto; margin-right:auto;"/>


## Debug issue

IntelliJ IDEA version 2021.3.1 and beyond might give exception error if you try to run in debug mode .In order to solve this issue go to this option windows : File -> Settings -> Build, Execution, Deployment -> Debugger -> Async Stack Traces and uncheck Instrumenting agent option.
