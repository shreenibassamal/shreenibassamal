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
