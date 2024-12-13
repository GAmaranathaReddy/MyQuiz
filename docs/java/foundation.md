# Java Basics - Quiz

## Question 1
What is the output of the following code snippet?

```java
System.out.println("Hello, Java!");
```

- <input type="radio" name="q1" value="0"> Java, Hello!
- <input type="radio" name="q1" value="1"> Hello, Java!
- <input type="radio" name="q1" value="0"> Compile Error
- <input type="radio" name="q1" value="0"> Runtime Error

---

## Question 2
Which of the following is a reserved keyword in Java?

- <input type="radio" name="q2" value="1"> `class`
- <input type="radio" name="q2" value="0"> `Main`
- <input type="radio" name="q2" value="0"> `variable`
- <input type="radio" name="q2" value="0"> `constant`

---

## Submit Quiz
<button onclick="calculateScore()">Submit</button>

## Your Score:
<div id="score"></div>

<script>
function calculateScore() {
    let score = 0;
    const questions = document.querySelectorAll('input[type="radio"]:checked');
    questions.forEach((question) => {
        score += parseInt(question.value);
    });
    document.getElementById("score").innerText = `Your total score is: ${score} / ${questions.length}`;
}
</script>
