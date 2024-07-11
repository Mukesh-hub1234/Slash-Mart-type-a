

def add_task():
    task = input("Enter a task: ")
    tasks.append(task)
    print("Task added!")

def complete_task():
    task = input("Enter a task to complete: ")
    if task in tasks:
        tasks.remove(task)
        print("Task completed!")
    else:
        print("Task not found!")

def remove_task():
    task = input("Enter a task to remove: ")
    if task in tasks:
        tasks.remove(task)
        print("Task removed!")
    else:
        print("Task not found!")

def list_tasks():
    print("Tasks:")
    for task in tasks:
        print(task)

while True:
    print("\n1. Add Task")
    print("2. Complete Task")
    print("3. Remove Task")
    print("4. List Tasks")
    print("5. Quit")
    choice = input("Choose an option: ")
    
    if choice == "1":
        add_task()
    elif choice == "2":
        complete_task()
    elif choice == "3":
        remove_task()
    elif choice == "4":
        list_tasks()
    elif choice == "5":
        break
    else:
        print("Invalid choice!")



