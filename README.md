def get_average(activity1, activity2, activity3):
    return (activity1 + activity2 + activity3) / 3

num_students = int(input("How many students will be processed? "))

for i in range(1, num_students + 1):
    print(f"\nStudent {i}")
    
    name = input("Enter name: ")
    
    
    activity1 = int(input("Activity 1: "))
    activity2 = int(input("Activity 2: "))
    activity3 = int(input("Activity 3: "))
    
    
    average = get_average(activity1, activity2, activity3)
    
    
    if average >= 90:
        status = "Excellent"
    elif average >= 80:
        status = "Very Good"
    elif average >= 75:
        status = "Passed"
    else:
        status = "Failed"
        
    
    print(f\"average: {average:.2f}")
    print(f"Status: {status}")
