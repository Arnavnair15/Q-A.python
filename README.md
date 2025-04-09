# List of questions with options and correct answers
questions = [
    {
        "question": "What is the capital of France?",
        "options": ["Paris", "London", "Berlin", "Madrid"],
        "answer": "Paris"
    },
    {
        "question": "Which planet is known as the Red Planet?",
        "options": ["Earth", "Mars", "Jupiter", "Saturn"],
        "answer": "Mars"
    },
    {
        "question": "What is the largest ocean on Earth?",
        "options": ["Atlantic Ocean", "Indian Ocean", "Arctic Ocean", "Pacific Ocean"],
        "answer": "Pacific Ocean"
    }
]

score = 0

print("Welcome to the Quiz Game!")
print("Good Luck!\n")

# Loop through each question
for q in questions:
    print(q["question"])
# Display options
    for i, option in enumerate(q["options"], 1):
        print(f"{i}. {option}")
    
# Get user's answer
    answer = input("Enter the correct answer: ")
    
# Check if the answer is correct
    if answer.lower() == q["answer"].lower():
        print("Correct!\n")
        score += 1
    else:
        print(f"Incorrect. The correct answer was: {q['answer']}\n")

# Display final score
print(f"Quiz finished! Your score: {score}/{len(questions)}")
