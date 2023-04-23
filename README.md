Download Link: https://assignmentchef.com/product/solved-assignment-1-cs440
<br>
The assignment is to be turned in before Midnight (by 11:59pm) on January 19th. You should turn in the solutions to this assignment as a PDF file through Canvas. The solutions should be produced using editing software programs, such as LaTeX or Word, otherwise they will not be graded. The assignment should be done in groups of two students. Each group must submit only one file that contains the full name, OSU email, and ONID of every member of the group.

<strong>1: Relational Model and SQL (10 points)</strong>

Consider the following relational schema:

Emp(<em>eid</em>:integer, <em>ename</em>:string, <em>age</em>:integer, <em>salary</em>:real)

Works(<em>eid</em>:integer, <em>did</em>:integer, <em>pc time</em>:integer)

Dept(<em>did</em>:integer, <em>dname</em>:string, <em>budget</em>:real, <em>managerid</em>:integer)

The underlined attributes are keys for their relations. Note that a manager is an employee as well and their manager id and employee id are the same. An employee can work in more than one department. The pct time field of the Works relation shows the percentage of time that a given employee works in a given department and is always greater than zero.

<table width="158">

 <tbody>

  <tr>

   <td width="158">dname</td>

  </tr>

  <tr>

   <td width="158">Business Development</td>

  </tr>

 </tbody>

</table>

A database sample (sample db.sql) is provided with this assignment and the output of the correct queries over this sample database is given in each part of this question. We have created an account for each student on the MySQL server of our department. The access guide to the MySQL server (database access guide.txt) is also posted with this assignment. You can import the sample database to your account on the MySQL server and use it to ensure that your queries are correct. You do not need to submit any .sql file in your assignment submission and must write your final SQL query in the single PDF file that you submit for all questions in this assignment.

Write the following queries in SQL. You should <em>not </em>submit any .sql file in your assignment submission and must write your final SQL queries in the single PDF file that you submit for all questions in this assignment.

<ul>

 <li>Return the <em>did </em>and <em>dname </em>of the departments with at least one half-time (50%) employee. (1 point)</li>

</ul>

The answer on the sample database is:

<table width="114">

 <tbody>

  <tr>

   <td width="36">did</td>

   <td width="77">dname</td>

  </tr>

  <tr>

   <td width="36">8</td>

   <td width="77">Hardware</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Print the names of every employee who works in ”Hardware”, ”Software”, and ”Research” departments. (1 point)</li>

</ul>

The answer on the sample database is:

<table width="152">

 <tbody>

  <tr>

   <td width="152">ename</td>

  </tr>

  <tr>

   <td width="152">Shirish Ossenbruggen</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Return the names of every department without any employee. (1 point) The answer on the sample database is:</li>

 <li>Print the <em>managerids </em>of managers who manage only departments with budgets greater than $5 million. (1 point)</li>

</ul>

The answer on the sample database is:

<table width="82">

 <tbody>

  <tr>

   <td width="82">managerid</td>

  </tr>

  <tr>

   <td width="82">110511</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Print the name of employees whose salary is less than or equal to the salary of every employee. (1 point)</li>

</ul>

The answer on the sample database is:

<table width="122">

 <tbody>

  <tr>

   <td width="122">ename</td>

  </tr>

  <tr>

   <td width="122">Antonio Lavante</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Print the <em>enames </em>of managers who manage the departments with the largest budget. (1 point) The answer on the sample database is:</li>

</ul>

<table width="139">

 <tbody>

  <tr>

   <td width="139">ename</td>

  </tr>

  <tr>

   <td width="139">Tonny Butterworth</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Print the name of every department and the average salary of the employees of that department. The department must have a budget more than or equal to $ (1 point) The answer on the sample database is:</li>

</ul>

<table width="298">

 <tbody>

  <tr>

   <td width="130">dname</td>

   <td width="168">average employee salary</td>

  </tr>

  <tr>

   <td width="130">Software</td>

   <td width="168">48291</td>

  </tr>

  <tr>

   <td width="130">Human Resources</td>

   <td width="168">717092.5</td>

  </tr>

  <tr>

   <td width="130">Research</td>

   <td width="168">490439.6666666667</td>

  </tr>

  <tr>

   <td width="130">Hardware</td>

   <td width="168">61842.125</td>

  </tr>

  <tr>

   <td width="130">Customer Service</td>

   <td width="168">40000</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Print the <em>managerids </em>of managers who control the largest amount of total budget. As an example, if a manager manages two departments, the amount of total budget for him will be the sum of budgets of two departments. We want to find managers that have max total budget. (1</li>

</ul>

point)

<table width="82">

 <tbody>

  <tr>

   <td width="82">managerid</td>

  </tr>

  <tr>

   <td width="82">111692</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Print the name of every employee whose salary is less than or equal to the average salary of all employees in his/her departments. (1 point) The answer on the sample database is:</li>

</ul>

ename

<table width="152">

 <tbody>

  <tr>

   <td width="152">Alex Dalas</td>

  </tr>

  <tr>

   <td width="152">Antonio Lavante</td>

  </tr>

  <tr>

   <td width="152">Tonny Conner</td>

  </tr>

  <tr>

   <td width="152">Shirish Ossenbruggen</td>

  </tr>

  <tr>

   <td width="152">DeForest Hagimont</td>

  </tr>

  <tr>

   <td width="152">Tonny Butterworth</td>

  </tr>

  <tr>

   <td width="152">Shigehito Kropatsch</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Print the name of every employee who works only in ”Hardware” department. (1 point) The answer on the sample database is:</li>

</ul>

ename

<table width="122">

 <tbody>

  <tr>

   <td width="122">Alex Dalas</td>

  </tr>

  <tr>

   <td width="122">Sergio Ravarez</td>

  </tr>

  <tr>

   <td width="122">Antonio Lavante</td>

  </tr>

  <tr>

   <td width="122">Tonny Conner</td>

  </tr>

  <tr>

   <td width="122">Gladys Cooper</td>

  </tr>

  <tr>

   <td width="122">Rodney Ferreri</td>

  </tr>

  <tr>

   <td width="122">Arie Staelin</td>

  </tr>

 </tbody>

</table>


