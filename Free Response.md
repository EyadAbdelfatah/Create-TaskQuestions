# 2024 AP Computer Science Principles Free-Response Questions: Set 1

## AP® Computer Science Principles Written Response Prompts

### Instructions:

- **Time:** 1 hour
- **Questions:** 2
- Read each question carefully and completely.
- Write your response in the space provided for each question in the Written Response booklet.
- You may plan your answers in this orange booklet, but no credit will be given for anything written in this booklet. You will only earn credit for what you write in the separate Written Response booklet.

---

### Pre-FRQ Practice

Butters the goat

```JavaScript
const resetHistory = function () {
  DOMSelectors.mainOutput.innerHTML = ""; // Clear previous quote
  if (quoteCurrent.length > 0) { //selection
    for (let i = 0; i < quoteCurrent.length; i++) { //iteratuion
      const quote = quoteCurrent[i];
      createQuoteCard(quote);
    }
  }
};//sequencing

```

Angelina:

```JavaScript
function insertText(inputContent, type) {
  DOMSelect.results.insertAdjacentHTML("beforeend", `<br></br>`);
  const content = inputContent;
  if (type === "file") {//selectiuon
    content.forEach(function (item) {//iteratin
      DOMSelect.results.insertAdjacentHTML(
        "beforeend",
        `<p class="text">${item}</p>`
      );
    });
  } else {//selectiopn
    content.forEach(function (item) {//iteration
      DOMSelect.results.insertAdjacentHTML(
        "beforeend",
        `<p class="text">${item.textContent}</p>`
      );
    });
    DOMSelect.input.innerHTML = "";
  }
  DOMSelect.inputbox.style.display = "none";
  DOMSelect.settings.style.display = "";//sequenciong
}
```

## Identify the Algorithm present in the JavaScript Files.

### Aspects of Algorithm

Sequencing
Selection
Iteration

### Question 1

Programs accept input to achieve their intended functionality. **Describe at least one valid input to your program and what your program does with that input.**

- Write your responses to this question only on the designated pages in the separate Written Response booklet.
- If there are multiple parts to this question, write the part letter with your response.
  Butters the goat

```JavaScript
DOMSelectors.generalForm.addEventListener(
  "submit",
  function quoteInitiate(userSubmit) {
    userSubmit.preventDefault();
    const valueUserAge = encodeURIComponent(DOMSelectors.userAge.value); // Test for displaying user Age: young / old
    const valueUserFeeling = encodeURIComponent(DOMSelectors.userFeeling.value); // Test for displaying user feeling: one of the options
    let category = "";

    if (valueUserAge === "young") {
      console.log(
        "You still have a long life ahead of you) Look what is out there!"
      );
    } else {
      console.log(
        "Focus on furthering your friendships. Appreciate the small things in life."
      );
    }
    categorySet();
    function categorySet() {
      if (valueUserFeeling === "Happy") {
        category = "happiness";
      } else if (valueUserFeeling === "Sad") {
        category = "alone";
      } else if (valueUserFeeling === "Scared") {
        category = "fear";
      } else if (valueUserFeeling === "Bored") {
        category = "attitude";
      } else if (valueUserFeeling === "Angry") {
        category = "anger";
      }
    }
    retrieveFeelingQuote(category); //Based on category, a specific quote is retrieve
  }
);
```

code uses the input to set a category based on the user input, the program then retrieves a quote based on the category of tjhe input

Angelina:

```JavaScript
function insertText(inputContent, type) {
  DOMSelect.results.insertAdjacentHTML("beforeend", `<br></br>`);
  const content = inputContent;
  if (type === "file") {
    content.forEach(function (item) {
      DOMSelect.results.insertAdjacentHTML(
        "beforeend",
        `<p class="text">${item}</p>`
      );
    });
  } else {
    content.forEach(function (item) {
      DOMSelect.results.insertAdjacentHTML(
        "beforeend",
        `<p class="text">${item.textContent}</p>`
      );
    });
    DOMSelect.input.innerHTML = "";
  }
  DOMSelect.inputbox.style.display = "none";
  DOMSelect.settings.style.display = "";
}
```

function takes the inputed content to see whether it was a file or not and based on that,

### Question 2

Refer to your Personalized Project Reference when answering this question.

#### Part (a):

Consider the first iteration statement included in the Procedure section of your Personalized Project Reference. **Describe what is being accomplished by the code in the body of the iteration statement.**

#### Part (b):

Consider the procedure identified in part (i) of the Procedure section of your Personalized Project Reference.

- Write two calls to your procedure that each cause a different code segment in the procedure to execute.
- Describe the expected behavior of each call. If it is not possible for two calls to your procedure to cause different code segments to execute, explain why this is the case for your procedure.

#### Part (c):

Suppose another programmer provides you with a procedure called `checkValidity(value)` that:

- Returns `true` if a value passed as an argument is considered valid by the other programmer.
- Returns `false` otherwise.

Using the list identified in the List section of your Personalized Project Reference, **explain in detailed steps an algorithm that uses `checkValidity` to check whether all elements in your list are considered valid by the other programmer.** Your explanation must be detailed enough for someone else to write the program code for the algorithm that uses `checkValidity`.

- Write your responses to this question only on the designated pages in the separate Written Response booklet.
- If there are multiple parts to this question, write the part letter with your response.

---

### End of Exam
