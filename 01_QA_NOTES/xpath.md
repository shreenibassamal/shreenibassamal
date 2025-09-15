
## Link for practice Xpath Below

## [Click on Link](https://xpath-by-shreenibas.netlify.app/)

XPath functions are used to **navigate XML/HTML documents** and **perform operations on nodes and values**.

---

## **1\. String Functions**

| Function | Description | Example |
| --- | --- | --- |
| `contains(string, substring)` | Checks if `string` contains `substring` | `//input[contains(@id,'user')]` |
| `starts-with(string, prefix)` | Checks if `string` starts with `prefix` | `//a[starts-with(@href,'https')]` |
| `ends-with(string, suffix)` | Checks if `string` ends with `suffix` (XPath 2.0) | `//a[ends-with(@href,'.com')]` |
| `string-length(string)` | Returns length of string | `string-length(//input/@value)` |
| `normalize-space(string)` | Removes leading/trailing spaces & normalizes spaces | `normalize-space(//div[@id='desc'])` |
| `substring(string, start, length)` | Extracts substring | `substring('HelloWorld',1,5)` → `Hello` |
| `substring-before(string, substring)` | Returns substring before a value | `substring-before('`[`user@example.com`](mailto:user@example.com)`','@')` → `user` |
| `substring-after(string, substring)` | Returns substring after a value | `substring-after('`[`user@example.com`](mailto:user@example.com)`','@')` → [`example.com`](http://example.com) |
| `translate(string, chars1, chars2)` | Replace characters | `translate('abc','a','x')` → `xbc` |
| `concat(string1, string2,...)` | Concatenate strings | `concat('Hello',' ','World')` → `Hello World` |
| `string(object)` | Converts object to string | `string(//div[@class='title'])` |

---

## **2\. Numeric Functions**

| Function | Description | Example |
| --- | --- | --- |
| `number(string)` | Converts string to number | `number('123')` → 123 |
| `sum(node-set)` | Returns sum of node values | `sum(//price)` |
| `floor(number)` | Rounds down | `floor(3.7)` → 3 |
| `ceiling(number)` | Rounds up | `ceiling(3.2)` → 4 |
| `round(number)` | Rounds to nearest integer | `round(3.5)` → 4 |

---

## **3\. Boolean Functions**

| Function | Description | Example |
| --- | --- | --- |
| `boolean(object)` | Converts object to boolean | `boolean(//div[@id='desc'])` |
| `not(expression)` | Negates boolean | `not(@disabled)` |
| `true()` | Returns boolean true | `//input[@enabled=true()]` |
| `false()` | Returns boolean false | `//input[@checked=false()]` |
| `lang(string)` | Checks language of node | `//p[lang('en')]` |

---

## **4\. Node Functions**

| Function | Description | Example |
| --- | --- | --- |
| `last()` | Returns last node position | `//li[last()]` |
| `position()` | Returns position of current node | `//li[position()=2]` |
| `count(node-set)` | Returns number of nodes | `count(//div)` |
| `name(node)` | Returns node name | `name(//div)` → `div` |
| `local-name(node)` | Returns local name without namespace | `local-name(//ns:div)` → `div` |
| `namespace-uri(node)` | Returns namespace URI | `namespace-uri(//ns:div)` |

---

## **5\. Date & Time Functions** (XPath 2.0)

| Function | Description | Example |
| --- | --- | --- |
| `current-date()` | Returns current date | `current-date()` → 2025-09-15 |
| `current-time()` | Returns current time | `current-time()` → 14:30:00 |
| `current-dateTime()` | Returns current date & time | `current-dateTime()` |
| `years-from-duration(duration)` | Extract years from duration | `years-from-duration(xs:dayTimeDuration('P3Y2M'))` → 3 |
| `days-from-duration(duration)` | Extract days | `days-from-duration(xs:dayTimeDuration('P3DT5H'))` → 3 |

---

## **6\. XPath Axes (Related to functions)**

While not functions per se, axes are **used in combination with XPath functions**:

| Axis | Description | Example |
| --- | --- | --- |
| `ancestor` | Selects parent nodes | `//span/ancestor::div` |
| `descendant` | Selects child/grandchild nodes | `//div/descendant::p` |
| `following-sibling` | Siblings after current node | `//h2/following-sibling::p` |
| `preceding-sibling` | Siblings before current node | `//h2/preceding-sibling::p` |
| `self` | Select current node | `//div/self::div` |
| `parent` | Select parent | `//span/parent::div` |

---

## **7\. Combining Functions (Examples)**

1. **Find element containing text and trimmed spaces**:
    

```xml
//div[normalize-space(text())='Login']
```

2. **Check last element with partial text**:
    

```xml
(//li[contains(text(),'Option')])[last()]
```

3. **Dynamic XPath using substring**:
    

```xml
//span[substring(@id,1,5)='user_']
```

4. **Check element with translated value**:
    

```xml
//input[translate(@type,'ABCDEFGHIJKLMNOPQRSTUVWXYZ','abcdefghijklmnopqrstuvwxyz')='text']
```

---

✅ **Summary**:

* **String functions:** `contains`, `starts-with`, `substring`, `normalize-space`, etc.
    
* **Numeric functions:** `sum`, `floor`, `ceiling`, `round`
    
* **Boolean functions:** `boolean`, `not`, `true()`, `false()`
    
* **Node functions:** `last()`, `position()`, `count()`, `name()`
    
* **Date/Time functions:** `current-date()`, `current-time()` (XPath 2.0)
    
* **Axes** are used to navigate the XML tree.

**Q1. What is XPath? Types?**  
XPath is a query language to locate nodes in XML/HTML.

Types: **Absolute** (`/html/body/div[2]/a`) and **Relative** (`//a[@id='login']`). Prefer relative in tests.

**Q2. CSS vs XPath?**

* **Speed:** CSS often faster.
    
* **Features:** XPath supports **axes**, **text()**, traversal **upwards** (to parent/ancestor); CSS cannot move up.
    
* **Readability:** CSS simpler; XPath more powerful for complex DOMs.
    

**Q3. XPath versions used in Selenium?**  
Selenium relies on browser engines (mostly **XPath 1.0**). Don’t expect 2.0/3.0 functions.

**Q4. Indexing start?**  
XPath indexes are **1-based**: `//li[1]` is the first `<li>`.

**Q5. What is a predicate?**  
Filter in square brackets: `//input[@type='email'][@required]`.

---

# Frequently used XPath patterns

**Attributes**

* Exact match: `//input[@name='q']`
    
* Multiple attrs: `//button[@type='submit' and @disabled]`
    
* Contains: `//div[contains(@class,'error')]`
    
* Starts with: `//a[starts-with(@id,'user_')]`
    
* Ends with (simulate): `//img[substring(@src, string-length(@src)-3) = '.png']`
    

**Text**

* Exact: `//button[text()='Login']`
    
* Contains text: `//h1[contains(normalize-space(.),'Welcome')]`
    
* Case-insensitive (simulate):  
    `//a[contains(translate(., 'ABCDEFGHIJKLMNOPQRSTUVWXYZ','abcdefghijklmnopqrstuvwxyz'), 'privacy')]`
    

**Hierarchy & position**

* Child: `//ul[@id='menu']/li/a`
    
* Any descendant: `//form//input[@type='password']`
    
* Nth item: `//ul[@id='menu']/li[3]`
    
* Last item: `//table//tr[last()]`
    
* First two: `//div[@role='row'][position()<=2]`
    

**Axes (traversal)**

* Parent: `//span[@class='price']/parent::div`
    
* Ancestor: `//input[@id='email']/ancestor::form`
    
* Following-sibling: `//label[.='Email']/following-sibling::input[1]`
    
* Preceding-sibling: `//td[.='Total']/preceding-sibling::td[1]`
    
* Descendant: `//section[@id='cart']/descendant::button[@type='submit']`
    
* Self: `//a[@data-test='x']/self::a`
    

**Unions & grouping**

* Either/or: `//input[@type='email'] | //input[@name='email']`
    
* Group conditions: `//a[(contains(@class,'btn') or @role='button') and not(@disabled)]`
    

**Dynamic IDs & classes**

* Stable part: `//*[contains(@id,'react-select') and contains(@id,'input')]`
    
* CSS-like class match (avoid partial class collisions):  
    `//*[contains(concat(' ', normalize-space(@class), ' '), ' btn-primary ')]`
    

**SVG/Canvas**

* SVG tag names need `local-name()` in HTML DOM:  
    `//*[local-name()='svg']//*[local-name()='path']`
    

**Shadow DOM (important!)**  
XPath **cannot** pierce shadow DOM. Use Selenium’s JS/shadow APIs instead.

**IFrames**  
Switch to frame first; XPath runs **inside** the current frame context.

**Namespaces (XML apps)**  
Use `local-name()` if prefixes vary: `//*[local-name()='book']`.

**Escaping quotes in string literals**  
Use `concat()` when your string has both quote types:  
`//a[@title=concat('He said "', "Hi", '" today')]`

---

# Real-world Selenium (Java) snippets

```java
// Single element
WebElement loginBtn = driver.findElement(By.xpath("//button[normalize-space()='Login']"));

// List + filter
List<WebElement> rows = driver.findElements(By.xpath("//table[@id='orders']//tr[position()>1]"));

// Robust class match
WebElement cta = driver.findElement(By.xpath("//*[contains(concat(' ', normalize-space(@class), ' '), ' btn-primary ')]"));

// Neighbor strategy
WebElement input = driver.findElement(By.xpath("//label[normalize-space()='Email']/following-sibling::input[1]"));

// Wait for clickable
WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(10));
WebElement save = wait.until(ExpectedConditions.elementToBeClickable(
    By.xpath("//button[.='Save' or .='Save changes']")));
```

---

# 30+ interview Qs with crisp answers

1. **Absolute vs Relative XPath?**  
    Absolute starts at root `/`; fragile. Relative starts with `//`; resilient.
    
2. **When to use contains() vs starts-with()?**  
    Use `contains()` for mid-string stability; `starts-with()` when prefix is stable (e.g., generated IDs).
    
3. **How do you locate by visible text ignoring extra spaces?**  
    `//tag[normalize-space(.)='Text']`.
    
4. **How to select the Nth occurrence of an element?**  
    `(//button[@type='button'])[3]`.
    
5. **Difference between** `.` and `text()`?  
    `.` = string value of the node (all descendant text); `text()` = direct text node child(ren).
    
6. **Select element by exact class token?**  
    `//*[contains(concat(' ', normalize-space(@class), ' '), ' chip ')]`.
    
7. **Find sibling cell based on header text in a table row.**  
    `//tr[td[normalize-space()='Email']]/td[2]`.
    
8. **Get row where a column matches and click its button.**  
    `//tr[td[normalize-space()='INV-123']]/td//button[normalize-space()='Pay']`.
    
9. **Pick last element**  
    `(//div[@role='option'])[last()]`.
    
10. **Find element by aria attributes (accessible apps).**  
    `//*[@aria-label='Search']` or `//*[@role='button' and @aria-pressed='true']`.
    
11. **Case-insensitive text search**  
    Use `translate()` trick (see above).
    
12. **Element inside iframe?**  
    `driver.switchTo().frame(WebElement frame)` then locate; switch back.
    
13. **Why avoid brittle XPaths like** `//div[3]/div[2]/span`?  
    Index-only paths break with DOM shifts; prefer attribute/text anchors.
    
14. **How to go from child to ancestor?**  
    `//span[@data-id='p']/ancestor::div[@role='row']`.
    
15. **Match elements with dynamic trailing numbers in id**  
    `//input[starts-with(@id,'user_')]`.
    
16. **Find label’s input when** `for` and `id` aren’t usable  
    `//label[.='Password']/following::input[1]` (scoped with a parent if possible).
    
17. **Select node by partial attribute and text together**  
    `//a[contains(@href,'terms') and contains(.,'Terms')]`.
    
18. **Click nth visible button when some are hidden**  
    Combine visibility check via WebDriver (not XPath) or filter with attributes like `not(contains(@style,'display:none'))`.
    
19. **Why** `normalize-space()` is useful?  
    Trims and condenses whitespace; stabilizes text matches.
    
20. **How to exclude nodes with** `not()`?  
    `//button[not(@disabled)]`.
    
21. **Union usage example**  
    `//input[@type='email'] | //input[@name='email']`.
    
22. **How to handle SVG icons?**  
    Use `local-name()` (see pattern above).
    
23. *Select element by data- attributes*\*  
    `//*[@data-testid='login']` — highly recommended for stable locators.
    
24. **What if attributes are completely dynamic?**  
    Anchor to **nearby stable text** and traverse with axes.
    
25. **Difference:** `//div[@id='x']//a` vs `//div[@id='x']/descendant::a`  
    Equivalent; the first is shorthand for `descendant::`.
    
26. **Pick second-to-last item**  
    `(//li)[last()-1]`.
    
27. **Click button following a specific heading**  
    `//h2[normalize-space()='Profile']/following::button[normalize-space()='Edit'][1]`.
    
28. **Locate input whose placeholder changes slightly**  
    `//input[contains(@placeholder,'search')]`.
    
29. **Is** `//*[@id='x']` bad?  
    Not inherently, but prefer [`By.id`](http://By.id)`("x")` if you have exact id—faster and clearer.
    
30. **Why prefer test IDs over XPath?**  
    Stability. Request `data-testid`/`data-qa` hooks from devs.
    
31. **How to find element by visible label when DOM nests them?**  
    `//label[normalize-space()='Country']//following::select[1]` (scope within a form/section).
    
32. **Get count of elements (for validation)**  
    Use WebDriver list size; XPath `count()` exists but not via By.xpath directly.
    
33. **Select link whose href ends with** `.pdf`  
    `//a[substring(@href, string-length(@href)-3) = '.pdf']`.
    

---

# Debugging & best practices

* Prefer **id/name/accessibility** locators first; use XPath when necessary.
    
* Add **scoping** to reduce ambiguity: `//form[@id='login']//input[@type='password']`.
    
* Avoid fragile index-only paths; use **attributes + text + axes**.
    
* Use **explicit waits** for dynamic UIs.
    
* For React/Angular, ask for **data-testid/data-qa** hooks.
    
* Avoid crossing **shadow DOM** with XPath—use shadow utilities.
    

# Mini practice (try mentally)

1. Select the price cell in the row where Product = “Laptop”.  
    `//tr[td[normalize-space()='Laptop']]/td[@data-col='price' or position()=3]`
    
2. Click the toggle right next to “Email Notifications”.  
    `//span[normalize-space()='Email Notifications']/following-sibling::input[@type='checkbox']`
    
3. Pick the “Delete” button inside the modal titled “Confirm”.  
    `//div[@role='dialog' and .//h2[normalize-space()='Confirm']]//button[normalize-space()='Delete']`
    

### Example of Dynamic Element

### Q- Write a Xpath to find the search-text field by using only id-attribute ?

Here we use **starts-with() and** by using **id-attribute and** the attribute value is start with **user\_ .**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1755596257331/16c1875f-4f84-4c61-8808-e9d06e2bd34a.png align="center")

### Q- Write a XPath to find the Products which price is graeter than 49.00.

Here we use **number()** to compare the number text which available inside the **&lt;td&gt;** tag.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1755665424518/f0135e1a-99ca-4e5f-8ad7-305fe38e1f16.png align="center")

### Q- Write a Xpath to find the product which invoice sl no is greater than INV-120.

Here we use **number()** to compare the number text which available inside the **&lt;td&gt;** tag but the text also contain String type text so we use **translate()** to remove the selected text.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1755666635567/1799ad09-c64a-4a43-8244-13b3a2427531.png align="center")

### Q- Write a Xpath to find

### Q- Write a Xpath to find

### Q- Write a Xpath to find
