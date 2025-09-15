## 🔹 **300 DQL Practice Questions (Topic-wise)**

---

## 1️⃣ Basic SELECT & Projection → **30 Questions**

1. Display all employees.
    
2. Show employee names and jobs.
    
3. List distinct job titles.
    
4. Display employee names and salaries with alias `Employee_Name`, `Monthly_Salary`.
    
5. Concatenate name and job.
    
6. Display first 3 letters of employee names.
    
7. List employees with dept numbers only.
    
8. Show job titles in uppercase.
    
9. Show employee names in lowercase.
    
10. Display all employee IDs.
    
11. Display employee IDs and names together.
    
12. Show employee names twice in the same row.
    
13. Display job and department numbers.
    
14. Show employee names with “EMP\_” prefix.
    
15. List employees with their employee number as string.
    
16. Show only department numbers (distinct).
    
17. Show all salaries.
    
18. Show salaries with a 10% bonus column.
    
19. Show salaries after 5% deduction.
    
20. Display annual salary (sal \* 12).
    
21. Display salary and commission (if any).
    
22. Display hire date only.
    
23. Display hire year only.
    
24. Display hire month only.
    
25. Display employee name with length of name.
    
26. Display employee name and ASCII value of first letter.
    
27. Show employee names with reversed text.
    
28. Display names padded with “\*”.
    
29. Show last 2 letters of employee names.
    
30. Show employee names without vowels.
    

---

## 2️⃣ Selection with WHERE → **30 Questions**

31. Show employees earning more than 2000.
    
32. Show employees earning less than 1500.
    
33. Employees in department 10.
    
34. Employees not in department 30.
    
35. Employees hired before 1981.
    
36. Employees hired after 1981.
    
37. Employees working as MANAGER.
    
38. Employees not working as SALESMAN.
    
39. Employees with commission not null.
    
40. Employees with commission null.
    
41. Employees whose salary is between 1000 and 2000.
    
42. Employees whose salary is not between 2000 and 3000.
    
43. Employees whose name starts with ‘S’.
    
44. Employees whose name ends with ‘N’.
    
45. Employees whose name has 5 letters.
    
46. Employees whose second letter is ‘A’.
    
47. Employees whose job contains ‘LER’.
    
48. Employees whose job is not CLERK or SALESMAN.
    
49. Employees hired in February.
    
50. Employees hired in December.
    
51. Employees hired on a Monday.
    
52. Employees with manager id = 7839.
    
53. Employees without a manager.
    
54. Employees earning same salary as 1250.
    
55. Employees earning more than employee SCOTT.
    
56. Employees working in dept 10 or 20.
    
57. Employees not working in dept 20 or 30.
    
58. Employees with empno &gt; 7900.
    
59. Employees with empno between 7600 and 7700.
    
60. Employees with name in (‘ALLEN’, ‘BLAKE’).
    

---

## 3️⃣ Sorting (ORDER BY) → **20 Questions**

61. Sort employees by name ascending.
    
62. Sort employees by name descending.
    
63. Sort employees by salary ascending.
    
64. Sort employees by salary descending.
    
65. Sort employees by job, then name.
    
66. Sort employees by deptno, then salary.
    
67. Sort employees by hire date oldest first.
    
68. Sort employees by hire date latest first.
    
69. Sort by commission nulls last.
    
70. Sort employees by empno.
    
71. Sort employees by length of name.
    
72. Sort employees by salary + commission.
    
73. Sort by department and job title.
    
74. Sort by reversed name.
    
75. Sort by last character of name.
    
76. Sort by job length.
    
77. Sort salaries in multiples of 100.
    
78. Sort employees by year of hire.
    
79. Sort employees by manager, then salary.
    
80. Sort by job descending, then name ascending.
    

---

## 4️⃣ Aggregate Functions → **30 Questions**

81. Count all employees.
    
82. Count distinct jobs.
    
83. Find max salary.
    
84. Find min salary.
    
85. Find avg salary.
    
86. Find sum of salaries.
    
87. Find total commission.
    
88. Find number of managers.
    
89. Find number of clerks.
    
90. Count employees in dept 10.
    
91. Count employees without commission.
    
92. Find max hire date.
    
93. Find min hire date.
    
94. Find difference between max and min salary.
    
95. Find stddev of salary (if supported).
    
96. Find variance of salary (if supported).
    
97. Count employees per manager.
    
98. Average salary per manager.
    
99. Highest salary per job.
    
100. Lowest salary per job.
    
101. Total salary + commission.
    
102. Max commission given.
    
103. Count of employees hired in 1981.
    
104. Count employees with name length &gt; 5.
    
105. Average salary of employees with commission.
    
106. Average salary of employees without commission.
    
107. Number of employees with job ‘SALESMAN’.
    
108. Maximum years worked by any employee.
    
109. Average years worked.
    
110. Total salary per hire year.
    

---

## 5️⃣ Group By & Having → **30 Questions**

111. Count employees per dept.
    
112. Avg salary per dept.
    
113. Max salary per dept.
    
114. Min salary per dept.
    
115. Sum salary per dept.
    
116. Count jobs per dept.
    
117. Avg commission per dept.
    
118. Count employees per job.
    
119. Max salary per job.
    
120. Count employees hired per year.
    
121. Count employees hired per month.
    
122. Count employees per manager.
    
123. Highest salary per manager.
    
124. Lowest salary per manager.
    
125. Average salary per hire year.
    
126. Departments with more than 3 employees.
    
127. Jobs with more than 2 employees.
    
128. Departments with avg salary &gt; 2000.
    
129. Jobs with avg salary &lt; 1500.
    
130. Managers with more than 2 subordinates.
    
131. Depts with total salary &gt; 8000.
    
132. Jobs with max salary &gt; 4000.
    
133. Departments with at least 1 clerk.
    
134. Depts with no salesman.
    
135. Count employees by commission status.
    
136. Count employees by job and dept.
    
137. Average salary per job per dept.
    
138. Max commission per job.
    
139. Total salary + commission per dept.
    
140. Departments with min salary &gt; 1000.
    

---

## 6️⃣ Joins → **30 Questions**

141. Show employee names with dept name.
    
142. Employee names with dept location.
    
143. Employees with their manager name.
    
144. Employees with dept and manager name.
    
145. All depts with employees.
    
146. All employees with dept (left join).
    
147. All depts with employees (right join).
    
148. Show employees without dept (outer join).
    
149. Show depts without employees.
    
150. Show employee and dept where dept is DALLAS.
    
151. Show employee and dept where dept is CHICAGO.
    
152. Show dept name and total employees.
    
153. Show dept name and avg salary.
    
154. Show dept name and highest paid employee.
    
155. Show dept name and lowest paid employee.
    
156. Show employee and dept location for dept 20.
    
157. Show employees and dept in same city.
    
158. Show manager with employees (self join).
    
159. Show employees without manager.
    
160. Show managers without subordinates.
    
161. Show employee and manager in same dept.
    
162. Show employees earning more than their manager.
    
163. Show dept name and all jobs inside.
    
164. Show employees grouped by dept name.
    
165. Show employee and dept name ordered by dept.
    
166. Show employee and dept location where loc = BOSTON.
    
167. Show depts in which KING works.
    
168. Show dept with no managers.
    
169. Show dept with no clerks.
    
170. Show all employees joined with all depts (cross join).
    

---

## 7️⃣ Subqueries → **30 Questions**

171. Employees earning more than avg salary.
    
172. Employees earning less than avg salary.
    
173. Employees earning equal to max salary.
    
174. Employees earning equal to min salary.
    
175. Employees working in same dept as SMITH.
    
176. Employees working in dept of KING.
    
177. Employees with salary &gt; BLAKE.
    
178. Employees hired after ALLEN.
    
179. Employees hired before SCOTT.
    
180. Employees earning more than any clerk.
    
181. Employees earning less than all managers.
    
182. Employees hired in same year as MILLER.
    
183. Employees earning same as JONES.
    
184. Employees in same dept as TURNER.
    
185. Employees with same job as MARTIN.
    
186. Employees who earn more than dept 30 avg.
    
187. Employees who earn less than dept 10 avg.
    
188. Employees who earn more than avg of their manager’s dept.
    
189. Depts with no employees.
    
190. Jobs with no employees.
    
191. Employees with commission &gt; avg commission.
    
192. Employees hired after company avg hire date.
    
193. Employees earning &gt; avg salary of managers.
    
194. Employees earning less than avg of clerks.
    
195. Depts where max salary &gt; company avg salary.
    
196. Employees working in depts in DALLAS.
    
197. Employees working in depts not in BOSTON.
    
198. Employees earning more than highest clerk.
    
199. Employees earning less than lowest manager.
    
200. Employees whose salary equals second highest.
    

---

## 8️⃣ Set Operators → **20 Questions**

201. List all employee names and dept names together.
    
202. List employees not working in dept table (if any).
    
203. List deptnos from both EMP and DEPT (union).
    
204. List deptnos common to EMP and DEPT.
    
205. List deptnos in EMP but not in DEPT.
    
206. List deptnos in DEPT but not in EMP.
    
207. List names of employees and managers (union).
    
208. List jobs from EMP and DEPT (dummy union).
    
209. Employees with salary &gt; 2000 UNION employees with job MANAGER.
    
210. Employees in dept 10 INTERSECT employees with job CLERK.
    
211. Employees in dept 20 MINUS employees with salary &lt; 2000.
    
212. Employees with commission UNION ALL employees with job SALESMAN.
    
213. Names of employees UNION names of depts.
    
214. Deptnos from EMP EXCEPT deptnos from DEPT.
    
215. Deptnos from DEPT EXCEPT deptnos from EMP.
    
216. Jobs in EMP INTERSECT (custom job list).
    
217. Salaries UNION commission.
    
218. Employees UNION managers self-join.
    
219. Employees INTERSECT subquery of high salary.
    
220. Employees MINUS employees with no commission.
    

---

## 9️⃣ String & Date Functions → **30 Questions**

221. Show employee name in uppercase.
    
222. Show employee name in lowercase.
    
223. Show employee name with first letter capital.
    
224. Show length of employee name.
    
225. Show reversed name.
    
226. Show ASCII of first character.
    
227. Show employee name without spaces.
    
228. Show employee name padded left.
    
229. Show employee name padded right.
    
230. Show substring of name (first 3 chars).
    
231. Show last 3 chars of name.
    
232. Show replace ‘A’ with ‘@’ in name.
    
233. Show concat of name and job.
    
234. Show employee name repeated twice.
    
235. Show names with vowels only.
    
236. Show names without vowels.
    
237. Show employees hired in 1981.
    
238. Show employees hired in February.
    
239. Show employees hired in December.
    
240. Show employees hired on Monday.
    
241. Show year of hiredate.
    
242. Show month of hiredate.
    
243. Show day of hiredate.
    
244. Show current date with employee info.
    
245. Show employees with sysdate - hiredate in days.
    
246. Show employees with years worked.
    
247. Show employees with months worked.
    
248. Show employees with weeks worked.
    
249. Show employees with hiredate + 100 days.
    
250. Show employees hired in last 10000 days.
    

---

## 🔟 CASE & Conditional Queries → **20 Questions**

251. Employees with salary grade High/Med/Low.
    
252. Employees with commission grade (None/Some).
    
253. Jobs renamed (Manager → Leader, Clerk → Support).
    
254. Department 10 renamed Accounting, 20 → Research.
    
255. Employees grouped as Old hire (before 1982) / New hire.
    
256. Employees salary bucketed by 1000s.
    
257. Employees with bonus eligibility (if salary &gt; 2000).
    
258. Employees with job category (Tech/Non-tech).
    
259. Employees with dept location tag.
    
260. Employees as “Managerial” vs “Non-Managerial”.
    

---

## 1️⃣1️⃣ Analytical / Window Functions → **30 Questions**

261. Rank employees by salary.
    
262. Dense rank employees by salary.
    
263. Row number employees by salary.
    
264. Rank employees by salary within dept.
    
265. Rank employees by hiredate.
    
266. Find 2nd highest salary using RANK.
    
267. Find 3rd highest salary using DENSE\_RANK.
    
268. Running total of salaries.
    
269. Running total of salaries per dept.
    
270. Moving average of salaries (3 rows).
    
271. Lag salary by 1 row.
    
272. Lead salary by 1 row.
    
273. Difference between salary and previous employee.
    
274. Employees with salary greater than previous employee.
    
275. First salary in each dept.
    
276. Last salary in each dept.
    
277. Nth salary in each dept.
    
278. Percent rank of salary.
    
279. Cumulative distribution of salary.
    
280. Employees with rank &lt;= 3 per dept.
    
281. Employee with highest salary per dept.
    
282. Employee with lowest salary per dept.
    
283. Top 2 employees per dept.
    
284. Show employees earning more than dept average (window).
    
285. Show employees earning less than dept average (window).
    
286. Employee with highest hiredate per dept.
    
287. Employee with earliest hiredate per dept.
    
288. Show employees with salary difference from dept avg.
    
289. Show employees with salary % of dept total.
    
290. Show employees with salary % of company total.
    

---

## 1️⃣2️⃣ Complex Business Queries → **10 Questions**

291. Show department with highest avg salary.
    
292. Show department with lowest avg salary.
    
293. Show employee with longest tenure.
    
294. Show employee with shortest tenure.
    
295. Show department with maximum headcount.
    
296. Show department with minimum headcount.
    
297. Show job with highest avg salary.
    
298. Show job with minimum avg salary.
    
299. Show department with no managers.
    
300. Show department with no clerks.
    

---

✅ This is a **complete 300-question DQL bank**, organized **topic-wise**.  
It starts from **easy SELECT** and goes all the way to **window functions and business queries**.
