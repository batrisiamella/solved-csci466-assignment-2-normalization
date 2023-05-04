Download Link: https://assignmentchef.com/product/solved-csci466-assignment-2-normalization
<br>
We discussed in class that a relational database designed in a poor way will allow for <em>anomalies </em>to occur. This is undesirable, so we use normalization to prevent them. Several relations are provided below, along with their functional dependencies. Answer the questions provided and fix what is broken. Perform only the current step for each question, i.e. when fixing 1NF, fix only 1NF, leaving the 2NF and 3NF violations alone until the question that asks about them.

<h2>TheQuestions</h2>

For each of the below, part (b) refers to the results of part (a), and part (c) refers to the results of part (b) – any changes made during the previous steps should be considered in the steps that follow. Each question is

worth 12 points.

<ol>

 <li><strong>Pharmacy</strong>(patient_id, patient_name, address, (Rx_num, trademark_name, generic_name, (filldate, num_refills_left), num_refills))</li>

</ol>

<strong>FunctionalDependencies:</strong>

<ul>

 <li>patient_id ⟶ patient_name, address</li>

 <li>patient_id, Rx_num ⟶ trademark_name, generic_name</li>

 <li>Rx_num ⟶ num_refills</li>

 <li>Rx_num, filldate ⟶ num_refills_left</li>

</ul>

<ol>

 <li>Is this relation in 1NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

 <li>Is this relation in 2NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

 <li>Is this relation in 3NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

</ol>

<ol start="2">

 <li><strong>Company</strong>(EmpID, EmpName, EmpAddr, (ProjID, ProjName, MgrID, MgrName, HoursWorked)) <strong>FunctionalDependencies:</strong>

  <ul>

   <li>EmpID ⟶ EmpName, EmpAddr</li>

   <li>ProjID ⟶ ProjName, MgrID, MgrName</li>

   <li>EmpID, ProjID ⟶ HoursWorked</li>

   <li>MgrID ⟶ MgrName</li>

  </ul></li>

</ol>

<ol>

 <li>Is this relation in 1NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

 <li>Is this relation in 2NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

 <li>Is this relation in 3NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

</ol>

<h2></h2>

<ol start="3">

 <li><strong>Property</strong>(id, county, lotNum, lotArea, price, taxRate, (datePaid, amount)) <strong>FunctionalDependencies:</strong>

  <ul>

   <li>id ⟶ county, lotNum, lotArea, price, taxRate</li>

   <li>lotArea ⟶ price</li>

   <li>county ⟶ taxRate</li>

   <li>id, datePaid ⟶ amount</li>

  </ul></li>

</ol>

<ol>

 <li>Is this relation in 1NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

 <li>Is this relation in 2NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

 <li>Is this relation in 3NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

</ol>

<ol start="4">

 <li><strong>StockExchange</strong>(Company, Symbol, HQ, Date, ClosePrice) <strong>FunctionalDependencies:</strong>

  <ul>

   <li>Symbol, Date ⟶ Company, HQ, ClosePrice</li>

   <li>Symbol ⟶ Company, HQ</li>

   <li>Symbol ⟶ HQ</li>

  </ul></li>

</ol>

<ol>

 <li>Is this relation in 1NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

 <li>Is this relation in 2NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

 <li>Is this relation in 3NF? If not, write an explanation of why it isn’t, then make the necessary changes to fix it.</li>

</ol>