document.getElementById("quizForm").addEventListener("submit", function(event) {
    event.preventDefault();

    let score = 0;

    // Check answers
    if (document.querySelector('input[name="q1"]:checked')?.value === "a noun") {
        score++;
    }
    if (document.querySelector('input[name="q2"]:checked')?.value === "doesn't") {
        score++;
    }

    // Add checks for other questions...

    // Show result
    document.getElementById("result").innerHTML = `Your score: ${score}`;
});
