# Loops
There are many different kinds of *loops*, but they all essentially do the same thing: **they repeat an action some number of times.**

<ul>

The statements for **loops** provided in *JavaScript* are:

<br>

<li> for statement</li>
<li>do...while statement</li>
<li> while statement</li>
<li>labeled statement</li>
<li>break statement</li>
<li>continue statement</li>
<li>for...in statement</li>
<li>for...of statement</li>

<br>

When a **for loop** executes, the following occurs:

for (initialization; condition; afterthought)
  statement


1. The initializing expression **initialization**, if any, **is executed.**This expression **usually initializes one or more loop counters**, but the syntax allows an expression of any degree of complexity. This expression can also **declare variables.**

2. Then the **condition expression is evaluated**. **If** the value of **condition is true, the loop statements execute**. **Otherwise,** the for **loop terminates.** (If the condition expression is omitted entirely, the **condition is assumed to be true.)**

3. The **statement** executes. To **execute multiple statements, use a block statement**({ }) to group those statements.

4. If present, the **update expression afterthought is executed.**

5. Control **returns to Step 2.**

>Examples: 

<br> 

 The function contains a for statement that counts the number of selected options in a scrolling list (a <select> element that allows multiple selections).

<form name="selectForm">
  <label for="musicTypes"
    >Choose some music types, then click the button below:</label
  >
  <select id="musicTypes" name="musicTypes" multiple>
    <option selected>R&B</option>
    <option>Jazz</option>
    <option>Blues</option>
    <option>New Age</option>
    <option>Classical</option>
    <option>Opera</option>
  </select>
  <button id="btn" type="button">How many are selected?</button>
</form>

Here, the for statement declares the variable i and initializes it to 0. It checks that i is less than the number of options in the <select> element, performs the succeeding if statement, and increments i by 1 after each pass through the loop.
<br>
 
 function countSelected(selectObject) {
  let numberSelected = 0;
  for (let i = 0; i < selectObject.options.length; i++) {
    if (selectObject.options[i].selected) {
      numberSelected++;
    }
  }
  return numberSelected;
}

const btn = document.getElementById("btn");

btn.addEventListener("click", () => {
  const musicTypes = document.selectForm.musicTypes;
  console.log(`You have selected ${countSelected(musicTypes)} option(s).`);
});


do while .. 

do
  statement
while (condition);


do until .. condition occurs ..




**Expressions and Operators**



 An *expression* is a valid unit of code that resolves to a value.
 
There are two types of expressions: those that have side effects (such as assigning values) and those that purely evaluate

 x=7 
is a example of a side effects assigning 


comparsions operators greater than less than eequal to
