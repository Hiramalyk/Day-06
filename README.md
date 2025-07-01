# Day-06
def get_grade(score):
    if 90 <= score <= 100:
        return "A"
    elif 85 <= score < 90:
        return "A-"
    elif 80 <= score < 85:
        return "B+"
    elif 70 <= score < 80:
        return "B"
    elif 60 <= score < 70:
        return "C"
    else:
        return "Fail"

def show_result(name="Student", score=0):
    if 0 <= score <= 100:
        grade = get_grade(score)
        print(f"{name} scored {score} → Grade: {grade}")
    else:
        print("Invalid score. Please enter a value between 0 and 100.")

show_result(name="Zara", score=87.5)
