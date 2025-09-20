# 1\. Git 🌀

## 1.1 What is Git? 📂

Git is a **distributed version control system**. It’s mainly used to:

* Track changes in code 📝
    
* Manage different versions of a project 🔀
    
* Allow multiple people to work on the same codebase at the same time without conflicts 👥
    

## 1.2 GitHub 🌐

GitHub is a **cloud-based platform** built on top of Git. It allows us to:

* Store repositories online ☁️
    
* Collaborate with team members 🤝
    
* Review code through pull requests 🔍
    
* Manage issues or tasks 📌
    

👉 **In short**: Git = Version Control ⚡ | GitHub = Collaboration Platform 🚀

---

## 1.3 My Project Experience 💼

In my projects, we used Git with GitHub:

* Created **branches** for new features or bug fixes 🌱
    
* Merged them into **main branch** via pull requests 🔄
    
* Handled **conflicts** when multiple people worked on the same files ⚔️
    
* Git helped us to **rollback changes**, **track history**, and improve collaboration ✅
    

---

## 1.4 Git Branching and Merging Workflow 🌳

| Step | Command / Action | Description |
| --- | --- | --- |
| 1 | `git init` | Initialize empty Git repository ⚡ |
| 2 | `git checkout -b b1` | Create and switch to branch `b1` 🌱 |
| 3 | Create `b1.txt` in Notepad ✍️ | Write one line in the file and save |
| 4 | `git add b1.txt` | Stage the file for commit 📦 |
| 5 | `git commit -m "Added b1.txt"` | Commit the file to `b1` branch ✅ |
| 6 | `git checkout -b b2` | Create and switch to branch `b2` 🌱 |
| 7 | Create `b2.txt` in Notepad ✍️ | Write one line in the file and save |
| 8 | `git add b2.txt` | Stage the file 📦 |
| 9 | `git commit -m "Added b2.txt"` | Commit the file to `b2` branch ✅ |
| 10 | `git checkout -b b3` | Create and switch to branch `b3` 🌱 |
| 11 | Create `b3.txt` in Notepad ✍️ | Write one line in the file and save |
| 12 | `git add b3.txt` | Stage the file 📦 |
| 13 | `git commit -m "Added b3.txt"` | Commit the file to `b3` branch ✅ |
| 14 | `git checkout master` | Switch back to master branch ⬅️ |
| 15 | `git merge b1` | Merge `b1` into master 🔀 |
| 16 | `git merge b2` | Merge `b2` into master 🔀 |
| 17 | `git merge b3` | Merge `b3` into master 🔀 |
| 18 | `git branch -d b1` | Delete branch `b1` 🧹 |
| 19 | `git branch -d b2` | Delete branch `b2` 🧹 |
| 20 | `git branch -d b3` | Delete branch `b3` 🧹 |
| 21 | `ls` / `cat b1.txt b2.txt b3.txt` | Verify all files are present in master 👀 |

---

## 1.5 Common Git Commands 🛠️

### 🔹 Repo Setup

| Command | Description |
| --- | --- |
| `git init` ⚡ | Initialize a new Git repository |
| `git clone <repo_url>` 🔗 | Clone an existing repository |

### 🔹 Configuration ⚙️

| Command | Description |
| --- | --- |
| `git config --global` [`user.name`](http://user.name) `"Name"` | Set username for all repos |
| `git config --global` [`user.email`](http://user.email) `"Email"` | Set email for all repos |

### 🔹 Status & Info 📋

| Command | Description |
| --- | --- |
| `git status` | Show working directory status |
| `git log` 📜 | Show commit history |
| `git log --oneline --graph --all` 🌳 | Compact history in tree format |
| `git diff` | Show unstaged changes |

### 🔹 Staging & Commit ✅

| Command | Description |
| --- | --- |
| `git add <file>` 📦 | Add file(s) to staging area |
| `git add .` | Stage all changes |
| `git commit -m "message"` | Commit staged changes |
| `git commit --amend` ✏️ | Edit last commit or add forgotten changes |

### 🔹 Branching 🌱

| Command | Description |
| --- | --- |
| `git branch` | List all branches |
| `git branch <name>` | Create a new branch |
| `git checkout <branch>` 🔄 | Switch to a branch |
| `git checkout -b <branch>` | Create and switch to new branch |
| `git switch <branch>` | Switch to a branch (new syntax) |
| `git switch -c <branch>` | Create & switch to new branch |

### 🔹 Merging 🔀

| Command | Description |
| --- | --- |
| `git merge <branch>` | Merge branch into current one |
| `git rebase <branch>` | Reapply commits on top of another branch |

### 🔹 Remote 🌍

| Command | Description |
| --- | --- |
| `git remote -v` | Show remote repositories |
| `git remote add origin <url>` | Add remote repo |
| `git push origin <branch>` 🚀 | Push branch to remote |
| `git push -u origin <branch>` | Push branch & set upstream |
| `git pull` ⬇️ | Fetch & merge from remote |
| `git fetch` | Download changes without merging |

### 🔹 Undo / Reset 🔄

| Command | Description |
| --- | --- |
| `git reset <file>` | Unstage a staged file |
| `git reset --hard <commit>` ⚠️ | Reset repo to specific commit |
| `git restore <file>` | Restore file from last commit |
| `git revert <commit>` | Create a commit that undoes changes |

### 🔹 Tagging 🏷️

| Command | Description |
| --- | --- |
| `git tag <name>` | Create a tag |
| `git tag` | List tags |
| `git push origin <tag>` | Push tag to remote |

### 🔹 Stash 📦

| Command | Description |
| --- | --- |
| `git stash` | Save changes temporarily |
| `git stash pop` | Reapply stashed changes |
| `git stash list` | Show stashed changes |

### 🔹 Clean Up 🧹

| Command | Description |
| --- | --- |
| `git branch -d <branch>` | Delete branch (safe) |
| `git branch -D <branch>` ❌ | Force delete branch |

---

✨ With Git + GitHub, collaboration becomes smooth, trackable, and efficient 🚀

# 2\. Maven ☕

## 2.1 What is Maven? 📂

Maven is a **build automation** and **project management** tool mainly used for Java projects. It helps to:

* Compile source code ⚙️
    
* Run tests ✅
    
* Package applications into JAR/WAR 📦
    
* Generate reports 📊
    
* Manage dependencies automatically 🔗
    

👉 Instead of manually adding JAR files, we declare them in `pom.xml` 📄 and Maven downloads them from the central repository. It also integrates well with **CI/CD pipelines like Jenkins** ⚡.

---

## 2.2 Real-time Usage 💼

* Installed & configured Maven in CMD 🖥️
    
* Declared dependencies in `pom.xml` 📄
    
* Configured **Surefire Plugin** for TestNG XML suites 🔧
    
* Ran scripts with:
    
    ```bash
    mvn clean test -P sts
    ```
    
* Checked reports in `target/surefire-reports` & `test-output` 📑
    

This helped us execute tests **without opening Eclipse** and integrate easily with **Jenkins pipelines** 🚀.

---

## 2.3 Maven Lifecycle Phases 🔄

| Phase | Command | Easy Meaning 📝 | Technical Meaning 🛠️ |
| --- | --- | --- | --- |
| Clean | `mvn clean` 🧹 | Delete old files, start fresh | Removes previous build outputs (e.g., `target/` folder) |
| Validate | `mvn validate` 🔍 | Check project setup | Ensures project structure & configuration are correct |
| Compile | `mvn compile` ⚙️ | Convert code to class files | Compiles `.java` → `.class` |
| Test | `mvn test` ✅ | Run tests | Executes unit/automation tests (JUnit, TestNG) |
| Package | `mvn package` 📦 | Make JAR/WAR file | Bundles compiled code + resources into `.jar`/`.war` |
| Verify | `mvn verify` 🔁 | Double-check build | Runs integration checks to ensure package is valid |
| Install | `mvn install` 💾 | Save build locally | Installs package into local repo (`~/.m2`) for use in other projects |
| Deploy | `mvn deploy` 🚀 | Share with team | Uploads package to remote repo (Nexus, Artifactory) |

---

## 2.4 Key `pom.xml` Tags 🏷️

| Tag Name | Easy Meaning 📝 | Technical Purpose |
| --- | --- | --- |
| `<profiles>` | Group of all profiles 📦 | Container for multiple `<profile>` definitions |
| `<profile>` | One profile (e.g., STS, Dev) | Defines build configuration |
| `<id>` | Profile name 🔑 | Used with `-P <id>` to activate profile |
| `<build>` | Build instructions 🔧 | Holds build-specific configs |
| `<plugins>` | List of plugins 🔌 | Groups multiple `<plugin>` |
| `<plugin>` | One specific plugin ⚡ | Defines plugin details (e.g., compiler) |
| `<groupId>` | Plugin’s org/group name 🏢 | Identifies publisher (e.g., `org.apache.maven.plugins`) |
| `<artifactId>` | Plugin name 🏷️ | Identifies plugin (e.g., `maven-compiler-plugin`) |
| `<version>` | Version of plugin 🔢 | Which version Maven uses |
| `<configuration>` | Custom settings ⚙️ | Defines options (e.g., `release=21`, test suite file) |
| `<release>` | Java version ☕ | Defines allowed Java version features |
| `<suiteXmlFiles>` | TestNG XML files 📂 | Surefire executes suites |
| `<suiteXmlFile>` | Single suite file 📄 | Exact path to XML suite (e.g., `Smoke.xml`) |

---

## 2.5 Example `pom.xml` ⚡

```xml
<build>
    <plugins>
        <!-- Compiler Plugin -->
        <plugin>
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-compiler-plugin</artifactId>
            <version>3.13.0</version>
            <configuration>
                <release>21</release>
            </configuration>
        </plugin>
    </plugins>
</build>

<profiles>
    <!-- Smoke Profile -->
    <profile>
        <id>smoke</id>
        <build>
            <plugins>
                <plugin>
                    <groupId>org.apache.maven.plugins</groupId>
                    <artifactId>maven-surefire-plugin</artifactId>
                    <version>3.2.5</version>
                    <configuration>
                        <suiteXmlFiles>
                            <suiteXmlFile>Smoke.xml</suiteXmlFile>
                        </suiteXmlFiles>
                    </configuration>
                </plugin>
            </plugins>
        </build>
    </profile>

    <!-- Integration Profile -->
    <profile>
        <id>integration</id>
        <build>
            <plugins>
                <plugin>
                    <groupId>org.apache.maven.plugins</groupId>
                    <artifactId>maven-surefire-plugin</artifactId>
                    <version>3.2.5</version>
                    <configuration>
                        <suiteXmlFiles>
                            <suiteXmlFile>Integration.xml</suiteXmlFile>
                        </suiteXmlFiles>
                    </configuration>
                </plugin>
            </plugins>
        </build>
    </profile>

    <!-- STS Profile -->
    <profile>
        <id>sts</id>
        <build>
            <plugins>
                <plugin>
                    <groupId>org.apache.maven.plugins</groupId>
                    <artifactId>maven-surefire-plugin</artifactId>
                    <version>3.2.5</version>
                    <configuration>
                        <suiteXmlFiles>
                            <suiteXmlFile>STS.xml</suiteXmlFile>
                        </suiteXmlFiles>
                    </configuration>
                </plugin>
            </plugins>
        </build>
    </profile>
</profiles>
```

---

## 2.6 Running Profiles 🏃‍♂️

```bash
mvn test -Psmoke
mvn test -Pintegration
mvn test -Psts
```

---

## 2.7 Example TestNG Suites 🧩

### 🔹 Smoke Suite

```xml
<!DOCTYPE suite SYSTEM "https://testng.org/testng-1.0.dtd" >
<suite name="SmokeSuite">
    <test name="SmokeTests">
        <classes>
            <class name="com.tests.LoginTest"/>
            <class name="com.tests.HomePageTest"/>
        </classes>
    </test>
</suite>
```

### 🔹 Integration Suite

```xml
<!DOCTYPE suite SYSTEM "https://testng.org/testng-1.0.dtd" >
<suite name="IntegrationSuite">
    <test name="IntegrationTests">
        <classes>
            <class name="com.tests.UserRegistrationTest"/>
            <class name="com.tests.PaymentTest"/>
            <class name="com.tests.OrderFlowTest"/>
        </classes>
    </test>
</suite>
```

### 🔹 STS Suite

```xml
<!DOCTYPE suite SYSTEM "https://testng.org/testng-1.0.dtd" >
<suite name="STSSuite">
    <test name="STSTests">
        <classes>
            <class name="com.tests.RegressionTest"/>
            <class name="com.tests.PerformanceTest"/>
        </classes>
    </test>
</suite>
```

# 3\. Jenkins ⚙️

## 3.1 What is Jenkins? 🌐

Jenkins is an **open-source automation server** mainly used for **Continuous Integration (CI)** and **Continuous Delivery (CD)** 🚀.

In my project:

* Integrated **Jenkins with Git & Maven** 🔗
    
* On each push, Jenkins:
    
    * Pulled latest code 📥
        
    * Compiled project using Maven ⚙️
        
    * Ran automated test cases ✅
        
    * Generated reports 📊
        

This automation ensured **fast feedback** and **seamless collaboration** among developers and testers.

---

## 3.2 Global Tool Configuration 🛠️

Global Tool Configuration allows us to define tools available for **all jobs**, avoiding repetitive setup.

| Tool | Purpose 📌 | How to Configure ⚙️ | Usage in Jobs 💡 |
| --- | --- | --- | --- |
| **JDK** ☕ | Java compiler for Jenkins & builds | Add name, set `JAVA_HOME`, or install automatically | Select JDK version in Build Environment |
| **Maven** 📦 | Build & dependency management tool | Add Maven version name, path, or auto-install | Jobs select Maven version in Build → `clean test` |
| **Git** 🌱 | Version control system | Add Git name & path to executable | Used for cloning/fetching repos |
| **Gradle** (optional) 📘 | Alternative build tool | Add Gradle name, path, or auto-install | Select Gradle if project uses it |
| **Ant** (optional) 🏗️ | Legacy Java build tool | Add Ant name, path, or auto-install | Select Ant for old projects |

👉 Navigate: **Manage Jenkins → Global Tool Configuration**

---

## 3.3 Creating a Jenkins Job 🧩

Steps to create a job:

| Step | Action 🎯 | Details / Notes 📝 |
| --- | --- | --- |
| 1 | Access Jenkins Dashboard | Open [`http://localhost:8080`](http://localhost:8080) & log in 🔑 |
| 2 | Click **New Item** | Start job creation ➕ |
| 3 | Enter Job Name | Unique name (e.g., *MyMavenProject*) 🏷️ |
| 4 | Select Project Type | Freestyle, Maven, or Pipeline ⚡ |
| 5 | Configure Source Code / POM | Git repo URL + credentials, or POM file path 📂 |
| 6 | Add Build Steps | e.g., `clean install`, shell scripts 🔧 |
| 7 | Configure Post-Build Actions | Email reports, archive artifacts, HTML reports 📬 |
| 8 | Save the Job | Store config 💾 |
| 9 | Run the Job | Click **Build Now** ▶️ |
| 10 | View Results | Build History & Console Output 📜 |

---

## 3.4 Jenkins Setup (Windows) 🖥️

| Step | Action ⚡ | Windows Instructions / Jenkins Action | Purpose ✅ |
| --- | --- | --- | --- |
| 1 | Install JDK ☕ | Download & install JDK → `C:\Program Files\Java\jdk-21` | Needed for Java, Maven, Jenkins, Selenium |
|  | Set Env Vars | Add `JAVA_HOME` + update PATH | Makes Java available system-wide |
|  | Verify | `java -version` | Confirms setup |
| 2 | Install Maven 📦 | Download & extract → `C:\apache-maven-3.9.6` | Needed to build Java projects |
|  | Set Env Vars | Add `MAVEN_HOME` + update PATH | Enables `mvn` commands |
|  | Verify | `mvn -v` | Confirms setup |
| 3 | Create Maven Project in Eclipse | `File → New → Maven Project` | Generates POM structure |
|  | Add Dependencies | Selenium, TestNG, Surefire 🔌 | Required libraries |
|  | Add `testng.xml` | Define suite & classes 🧩 | Select which tests run |
|  | Run in Eclipse | Right-click → `Run As TestNG Suite` | Verify before Jenkins integration |
| 4 | Install Jenkins | Download & install as **Windows Service** | Background automation tool |
|  | Start Jenkins | Open [`http://localhost:8080`](http://localhost:8080) | Access Jenkins Dashboard |
|  | Unlock Jenkins | Use key in `C:\Program Files\Jenkins\secrets` | First-time login 🔑 |
|  | Install Plugins | Select *Install Suggested Plugins* | Basic setup |
| 5 | Configure Tools | Add JDK & Maven under **Global Tool Config** | Allows Jenkins to use tools |
| 6 | Create Jenkins Job | New Item → Freestyle → *MySeleniumJob* | Create automation job |
|  | Add Build Step | `Invoke top-level Maven targets → clean test` | Run tests via Maven |
|  | Run Job | **Build Now** → View Console | Verify integration ✔️ |
| 7 | Configure Email Notifications 📧 | Install *Email Extension Plugin* | Send reports |
|  | SMTP Setup | Gmail SMTP → App password 🔐 | Jenkins can send mail |
|  | Post-Build Action | Editable Email Notification | Configure recipients & reports |
|  | Attach Reports | `**/test-output/emailable-report.html` | Send TestNG report 📑 |
|  | Trigger | Always | Send mail every build 📬 |
| 8 | Schedule Build ⏰ | Cron: `15 11 * * *` | Runs daily at 11:15 AM 🕚 |

---

## 3.5 Summary ✨

* Jenkins automates builds, tests, and reporting ⚡
    
* Ensures consistency via **Global Tool Config** 🛠️
    
* Supports **Freestyle, Maven, and Pipeline jobs** 🧩
    
* Integrated with **Git, Maven, TestNG** 🔗
    
* Configurable for **email reports, scheduled runs, CI/CD** 📬
* ---
* # 4\. Extent Reports 📊

## 4.1 What are Extent Reports? 🌐

Extent Reports is a **reporting library** widely used in automation testing with **Selenium + TestNG**. It generates **interactive, professional HTML reports** that are much more advanced than default TestNG reports.

✨ **Advantages of Extent Reports:**

* Step-by-step logging 📝
    
* Screenshots for failed steps 📸
    
* Customizable with themes 🎨
    
* Supports authors, categories, modules 🧑‍💻
    
* Consolidated view of entire suite 📂
    

👉 In my project, I used Extent Reports to log test steps, attach screenshots, and provide execution environment details.

---

## 4.2 Implementation in Framework ⚙️

Steps:

1. Create `ExtentSparkReporter` → define file path, theme, name 📑
    
2. Create `ExtentReports` object → attach reporter 🔗
    
3. Add **System Info** (OS, Browser, Tester) 💻
    
4. Create `ExtentTest` for each test 🎯
    
5. Log test steps with `Status` enums ✅❌⚠️
    
6. Call `flush()` → generate report 📊
    

---

## 4.3 Example Code 💻

import com.aventstack.extentreports.ExtentReports;

import com.aventstack.extentreports.ExtentTest;

import com.aventstack.extentreports.Status;

import com.aventstack.extentreports.reporter.ExtentSparkReporter;

import com.aventstack.extentreports.reporter.configuration.Theme;

import [java.util.Date](http://java.util.Date);

public class ExtentReportEnhanced {

public static void main(String\[\] args) {

// Step 1: Setup Spark Reporter with timestamp

String timeStamp = new Date().toString().replace(" ", "\_").replace(":", "\_");

String reportPath = "extentReport\_" + timeStamp + ".html";

ExtentSparkReporter spark = new ExtentSparkReporter(reportPath);

spark.config().setDocumentTitle("CRM Test Report");

spark.config().setReportName("Automation Execution Report");

spark.config().setTheme(Theme.DARK);

// Step 2: Create ExtentReports & attach reporter

ExtentReports extent = new ExtentReports();

extent.attachReporter(spark);

// Step 3: Add environment/system details

extent.setSystemInfo("OS", "Windows 10");

extent.setSystemInfo("Browser", "Chrome 122");

extent.setSystemInfo("Tester", "Saddam");

// Step 4: Create test and add logs

ExtentTest test = extent.createTest("Login Test");

test.log([Status.INFO](http://Status.INFO), "Browser launched successfully 🌐");

test.log(Status.PASS, "User logged in successfully ✅");

// Step 5: Generate the report

extent.flush();

System.out.println("Report generated at: " + reportPath);

}

}

---

# 5\. Exceptions & Their Solutions 🐞

In Selenium, exceptions are unexpected events that **disrupt test execution**. Java provides **try–catch** blocks for handling them.

| # | Exception ⚡ | When it Occurs ❌ | Solution ✅ |
| --- | --- | --- | --- |
| 1 | NoSuchElementException | Element not found | Check locator, use **explicit wait** ⏳ |
| 2 | ElementNotInteractableException | Element present but not clickable | Wait until visible / scroll 🔄 |
| 3 | StaleElementReferenceException | Element detached from DOM (reload) | Re-locate element after reload 🔁 |
| 4 | TimeoutException | Wait exceeded | Increase wait or correct condition ⏱️ |
| 5 | NoSuchFrameException | Switching to non-existing frame | Verify frame name/index 🪟 |
| 6 | NoAlertPresentException | Switching to non-existing alert | Ensure alert is triggered ⚠️ |
| 7 | ElementClickInterceptedException | Popup blocking click | Wait/scroll or use JS click 🖱️ |
| 8 | SessionNotCreatedException | Driver-browser mismatch | Update WebDriver/browser 🌍 |
| 9 | InvalidSelectorException | Invalid XPath/CSS | Fix locator syntax ✏️ |
| 10 | WebDriverException | Browser not reachable | Check setup & session 🔧 |
| 11 | FileNotFoundException | File path missing | Provide correct path 📂 |
| 12 | InvalidArgumentException | Invalid input/URL | Use valid URLs & paths 🔗 |

---

# 6\. Listeners 🎧

Listeners in **TestNG** are like **observers** 👀 that react to test events (start, pass, fail, skip).

✨ **Benefits:**

* Capture screenshots on failure 📸
    
* Auto-log results ✅❌⚠️
    
* Integrate with reports (Extent Reports) 📊
    

---

## 6.1 Implementation ⚡

### 🔹 Step 1: Create Listener Class

import org.testng.ITestListener;

import org.testng.ITestResult;

public class MyTestListener implements ITestListener {

@Override

public void onTestStart(ITestResult result) {

System.out.println("Test Started: " + result.getName());

}

@Override

public void onTestSuccess(ITestResult result) {

System.out.println("Test Passed: " + result.getName());

}

@Override

public void onTestFailure(ITestResult result) {

System.out.println("Test Failed: " + result.getName());

// ✅ Capture screenshot code here

}

@Override

public void onTestSkipped(ITestResult result) {

System.out.println("Test Skipped: " + result.getName());

}

}

### 🔹 Step 2: Attach Listener

**Option 1: TestNG XML**

&lt;suite name="Suite"&gt;

&lt;listeners&gt;

&lt;listener class-name="com.listeners.MyTestListener"/&gt;

&lt;/listeners&gt;

&lt;test name="Test"&gt;

&lt;classes&gt;

&lt;class name="com.tests.LoginTest"/&gt;

&lt;/classes&gt;

&lt;/test&gt;

&lt;/suite&gt;

**Option 2: @Listeners Annotation**

import org.testng.annotations.Listeners;

import org.testng.annotations.Test;

@Listeners(MyTestListener.class)

public class LoginTest {

@Test

public void testLoginPass() {

System.out.println("Login test executed successfully ✅");

}

@Test

public void testLoginFail() {

throw new RuntimeException("Forcing a failure ❌");

}

}

---

# 7\. TestNG Annotations 🧩

Annotations in TestNG control **test execution flow** ⏳.

| # | Annotation | Description |
| --- | --- | --- |
| 1 | @BeforeSuite | Runs before all tests 🏁 |
| 2 | @AfterSuite | Runs after all tests 🏁 |
| 3 | @BeforeTest | Runs before `<test>` in XML ⚡ |
| 4 | @AfterTest | Runs after `<test>` in XML ⚡ |
| 5 | @BeforeClass | Before first method in class 📘 |
| 6 | @AfterClass | After all methods in class 📘 |
| 7 | @BeforeMethod | Before each test method 🔄 |
| 8 | @AfterMethod | After each test method 🔄 |
| 9 | @Test | Marks a method as test case ✅ |
| 10 | @DataProvider | Provides test data 📊 |
| 11 | @Parameters | Pass values from XML 🔑 |
| 12 | @BeforeGroups | Before first method in group 📂 |
| 13 | @AfterGroups | After all methods in group 📂 |
| 14 | @Factory | Runs set of test classes 🏗️ |
| 15 | @Listeners | Attach listeners 🎧 |
| 16 | @Ignore | Skip test ❌ |
| 17 | @Test(invocationCount) | Run same test multiple times 🔁 |
| 18 | @Test(priority) | Define test order 🔢 |
| 19 | @Test(dependsOnMethods) | One test depends on another 🔗 |
| 20 | @Test(expectedExceptions) | Expected exception in test ⚡ |
* ---
* # 8️⃣ UtilityClassObject 🛠️

UtilityClassObject is designed to manage **WebDriver** and **ExtentTest** objects in a **thread-safe** way using `ThreadLocal`.  
This is 🔑 for **parallel execution** so tests don’t interfere with each other.

### ✅ Why use it?

* Each test gets its **own WebDriver** and **ExtentTest** instance.
    
* Prevents logs/screenshots from mixing up.
    
* Ensures **clean reports** in parallel runs.
    

public class UtilityClassObject {

public static ThreadLocal&lt;ExtentTest&gt; test = new ThreadLocal&lt;&gt;();

public static ThreadLocal&lt;WebDriver&gt; driver = new ThreadLocal&lt;&gt;();

public static ExtentTest getTest() { return test.get(); }

public static void setTest(ExtentTest actTest) { test.set(actTest); }

public static WebDriver getDriver() { return driver.get(); }

public static void setDriver(WebDriver actDriver) { driver.set(actDriver); }

}

👉 **Real-Time Use:**

* Call `setDriver()` in setup.
    
* Use `getDriver()` in test steps.
    
* Same approach for `ExtentTest` logging.
    

---

# 9️⃣ testng.xml 📄

`testng.xml` is like a **control file** for TestNG ⚡. It tells which test classes to run, order, groups, parallel execution, and parameters.

### 🎯 Benefits

* Runs multiple classes in sequence or parallel.
    
* Groups test cases (login, payment, regression).
    
* Adds parameters and listeners easily.
    

### 🏗️ Structure

| Tag / Attribute | Example | Purpose |
| --- | --- | --- |
| `<!DOCTYPE suite SYSTEM>` | Declared at top | Defines it as a TestNG file. |
| `<suite>` | `<suite name="Suite">` | Root element (whole suite). |
| `<test>` | `<test name="Test">` | A group of classes/tests. |
| `<classes>` | `<classes>...</classes>` | Container for test classes. |
| `<class>` | `<class name="com.tests.LoginTest"/>` | Runs that specific test class. |

&lt;!DOCTYPE suite SYSTEM "https://testng.org/testng-1.0.dtd" &gt;

&lt;suite name="Suite"&gt;

&lt;test name="Test"&gt;

&lt;classes&gt;

&lt;class name="com.tests.LoginTest"/&gt;

&lt;/classes&gt;

&lt;/test&gt;

&lt;/suite&gt;

👉 **Real-Time Use:** Helps centralize all test classes, reduces manual execution, and integrates smoothly with Jenkins.

---

# 🔟 Selenium Java Architecture 🏗️

Selenium Java follows **OOP concepts**: Abstraction, Inheritance, and Runtime Polymorphism.

### 🔑 Flow:

* **SearchContext** → Base interface (`findElement`, `findElements`).
    
* **WebDriver** → Extends SearchContext (browser-level methods).
    
* **RemoteWebDriver** → Implements WebDriver.
    
* **Browser Drivers** (ChromeDriver, FirefoxDriver) → Extend RemoteWebDriver.
    

| Component | Type | Contains | Inherits | Role |
| --- | --- | --- | --- | --- |
| SearchContext | Interface | `findElement()`, `findElements()` | — | Base interface |
| WebDriver | Interface | Browser-level methods | Extends SearchContext | Cross-browser automation |
| RemoteWebDriver | Class | Implements all methods | Implements WebDriver | Core implementation |
| ChromeDriver | Class | Chrome browser control | Extends RemoteWebDriver | Launch Chrome |
| FirefoxDriver | Class | Firefox browser control | Extends RemoteWebDriver | Launch Firefox |

WebDriver driver = new ChromeDriver(); // RTP: WebDriver reference, ChromeDriver object

👉 **Real-Time Use:** One code works for multiple browsers by just changing driver object creation.

---

# 1️⃣1️⃣ Screenshot 📸

Screenshots in Selenium help in 📊 **debugging, bug reporting, and attaching to reports**.

### 🎯 Types

1. **Element Screenshot** → Only captures specific element.
    
2. **Full Page Screenshot** → Captures entire browser window.
    

// Element Screenshot

WebElement logo = driver.findElement(By.id("logo"));

File src = logo.getScreenshotAs(OutputType.FILE);

FileHandler.copy(src, new File("./Screenshots/logo.png"));

// Full Page Screenshot

TakesScreenshot ts = (TakesScreenshot) driver;

File src = ts.getScreenshotAs(OutputType.FILE);

FileHandler.copy(src, new File("./Screenshots/full.png"));

| Code Part | Belongs To | Purpose |
| --- | --- | --- |
| `TakesScreenshot` | Interface | Capture screenshots |
| `(TakesScreenshot) driver` | Type Casting | Converts driver into TakesScreenshot |
| `getScreenshotAs()` | Method | Returns screenshot as file |
| `FileHandler.copy()` | Selenium IO | Saves screenshot permanently |

👉 **Real-Time Use:** Attach failed step screenshots to Extent Reports for clarity.

---

# 1️⃣2️⃣ Page Object Model (POM) 📘

POM separates **locators + actions** from test logic.  
Each page = One class 📄.

### 🎯 Benefits

* ✅ Reusable code.
    
* ✅ Easy maintenance.
    
* ✅ Centralized locators.
    

public class LoginPage {

WebDriver driver;

@FindBy(id = "username") private WebElement email;

@FindBy(name = "password") private WebElement password;

@FindBy(xpath = "//button\[text()='Login'\]") private WebElement loginBtn;

public LoginPage(WebDriver driver) {

this.driver = driver;

PageFactory.initElements(driver, this);

}

public void login(String user, String pass) {

email.sendKeys(user);

password.sendKeys(pass);

loginBtn.click();

}

}

👉 **Real-Time Use:** If login button changes, update only in LoginPage.java, not in all tests.

---

# 1️⃣3️⃣ WebDriver & WebElement Methods 🖥️

### 🌐 WebDriver Interface Methods

| Method | Return | Purpose | Example |
| --- | --- | --- | --- |
| get(url) | void | Opens URL | driver.get("https://google.com"); |
| getTitle() | String | Page title | driver.getTitle(); |
| getWindowHandle() | String | Current window ID | driver.getWindowHandle(); |
| switchTo() | TargetLocator | Switch control | driver.switchTo().alert(); |
| quit() | void | Closes all windows | driver.quit(); |

---

### 🖱️ WebElement Interface Methods

| Method | Example | Purpose |
| --- | --- | --- |
| click() | element.click(); | Click on element |
| sendKeys() | element.sendKeys("admin"); | Enter text |
| clear() | element.clear(); | Clear field |
| getText() | element.getText(); | Get visible text |
| isDisplayed() | element.isDisplayed(); | Check visibility |
| isEnabled() | element.isEnabled(); | Check if enabled |
| isSelected() | element.isSelected(); | Check checkbox/radio |

👉 **Real-Time Use:** `sendKeys()` for input, `click()` for buttons, `getText()` for validations.
---

* 
