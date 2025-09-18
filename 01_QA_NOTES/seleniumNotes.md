# 🟢 Selenium WebDriver – Classes & Interfaces (Java)

---

## 🔹 1. **Main Interfaces**

### 1.1 `WebDriver`

> Base interface for controlling browsers.  
> ✅ Implemented by `ChromeDriver`, `FirefoxDriver`, `EdgeDriver`, etc.

**Key Methods:**

* `get(String url)`
    
* `getTitle()`
    
* `getCurrentUrl()`
    
* `getPageSource()`
    
* `close()`
    
* `quit()`
    
* `findElement(By by)`
    
* `findElements(By by)`
    
* `getWindowHandle()`
    
* `getWindowHandles()`
    
* `switchTo()`
    
* `manage()`
    
* `navigate()`
    

---

### 1.2 `WebElement`

> Represents an element on the webpage.  
> ✅ Returned by `findElement()`.

**Key Methods:**

* `click()`
    
* `sendKeys(CharSequence… keys)`
    
* `clear()`
    
* `getText()`
    
* `getTagName()`
    
* `getAttribute(String name)`
    
* `isDisplayed()`
    
* `isEnabled()`
    
* `isSelected()`
    
* `submit()`
    
* `getCssValue(String propertyName)`
    
* `getRect()` (size & position)
    

---

### 1.3 `By`

> Locator class used to find elements.  
> ✅ Static methods:

* [`By.id`](http://By.id)`(String id)`
    
* [`By.name`](http://By.name)`(String name)`
    
* `By.className(String className)`
    
* `By.tagName(String tag)`
    
* `By.linkText(String text)`
    
* `By.partialLinkText(String partial)`
    
* `By.cssSelector(String css)`
    
* `By.xpath(String xpath)`
    

---

### 1.4 `Alert`

> Handle JavaScript popups.

**Key Methods:**

* `accept()`
    
* `dismiss()`
    
* `getText()`
    
* `sendKeys(String keys)`
    

---

### 1.5 `Navigation` (`driver.navigate()`)

* `to(String url)`
    
* `back()`
    
* `forward()`
    
* `refresh()`
    

---

### 1.6 `Options` (`driver.manage()`)

* `window()` → returns `Window` interface
    
* `timeouts()` → returns `Timeouts` interface
    
* `deleteAllCookies()`
    
* `deleteCookieNamed(String name)`
    

---

### 1.7 `Window` (sub-interface of Options)

* `maximize()`
    
* `minimize()`
    
* `fullscreen()`
    
* `setSize(Dimension size)`
    
* `getSize()`
    
* `setPosition(Point position)`
    
* `getPosition()`
    

---

### 1.8 `Timeouts`

* `implicitlyWait(Duration time)`
    
* `pageLoadTimeout(Duration time)`
    
* `scriptTimeout(Duration time)`
    

---

### 1.9 `TargetLocator` (`driver.switchTo()`)

* `frame(int index)`
    
* `frame(String nameOrId)`
    
* `frame(WebElement frameElement)`
    
* `parentFrame()`
    
* `defaultContent()`
    
* `alert()`
    
* `window(String handle)`
    

---

## 🔹 2. **Supporting Interfaces / Classes**

### 2.1 `TakesScreenshot`

* `getScreenshotAs(OutputType<T> target)`
    

---

### 2.2 `JavascriptExecutor`

* `executeScript(String script, Object... args)`
    
* `executeAsyncScript(String script, Object... args)`
    

---

### 2.3 `Actions` (Class)

Used for mouse & keyboard actions.

**Methods (all return** `Actions` so you can chain):

* `moveToElement(WebElement target)`
    
* `click()`
    
* `click(WebElement target)`
    
* `doubleClick()`
    
* `doubleClick(WebElement target)`
    
* `contextClick()`
    
* `contextClick(WebElement target)`
    
* `dragAndDrop(WebElement source, WebElement target)`
    
* `dragAndDropBy(WebElement source, int xOffset, int yOffset)`
    
* `keyDown(Keys key)`
    
* `keyUp(Keys key)`
    
* `sendKeys(CharSequence... keys)`
    
* `build()`
    
* `perform()`
    

---

### 2.4 `Select` (Class)

For dropdowns.

**Key Methods:**

* `selectByIndex(int index)`
    
* `selectByValue(String value)`
    
* `selectByVisibleText(String text)`
    
* `deselectByIndex(int index)`
    
* `deselectByValue(String value)`
    
* `deselectByVisibleText(String text)`
    
* `deselectAll()`
    
* `getOptions()`
    
* `getAllSelectedOptions()`
    
* `getFirstSelectedOption()`
    
* `isMultiple()`
    

---

### 2.5 `WebDriverWait` (extends FluentWait)

* `until(ExpectedCondition<T> condition)`
    

---

### 2.6 `FluentWait<T>`

* `withTimeout(Duration time)`
    
* `pollingEvery(Duration interval)`
    
* `ignoring(Class<? extends Throwable> exceptionType)`
    

---

### 2.7 `ExpectedConditions` (Class)

Common ready-made conditions:

* `visibilityOfElementLocated(By locator)`
    
* `elementToBeClickable(By locator)`
    
* `alertIsPresent()`
    
* `frameToBeAvailableAndSwitchToIt(By locator)`
    
* `titleIs(String title)`
    
* `urlContains(String fraction)`
    

---

### 2.8 `Keys` (Enum)

Keyboard keys.

* `Keys.ENTER`
    
* [`Keys.TAB`](http://Keys.TAB)
    
* `Keys.CONTROL`
    
* `Keys.ARROW_DOWN` etc.
    

---

## 🔹 3. **Driver Classes (implement WebDriver)**

* `ChromeDriver`
    
* `FirefoxDriver`
    
* `EdgeDriver`
    
* `SafariDriver`
    
* `InternetExplorerDriver` (deprecated)
    

All inherit WebDriver’s methods.

---

## 🔹 4. **Utility Classes**

* `Dimension` → window size (`new Dimension(1024, 768)`)
    
* `Point` → window position (`new Point(100, 200)`)
    
* `Rectangle` → element position + size
    
* `Cookie` → browser cookies handling
    

---

# ✅ Summary Table

| **Category** | **Classes/Interfaces** | **Example Methods** |
| --- | --- | --- |
| Browser Control | WebDriver | get(), close(), quit() |
| Elements | WebElement | click(), sendKeys(), getText() |
| Locators | By | id(), name(), xpath() |
| Navigation | Navigation | back(), forward(), refresh() |
| Alerts | Alert | accept(), dismiss(), getText() |
| Windows/Frames | TargetLocator | frame(), alert(), window() |
| Manage | Options, Window, Timeouts | maximize(), implicitlyWait() |
| Screenshot | TakesScreenshot | getScreenshotAs() |
| JS Execution | JavascriptExecutor | executeScript() |
| User Actions | Actions | dragAndDrop(), doubleClick() |
| Dropdown | Select | selectByValue(), getOptions() |
| Waits | WebDriverWait, FluentWait, ExpectedConditions | until(), visibilityOfElement() |
