---
toc: true
comments: false
layout: post
title: Algorithms Homework
description: Period 1 Algorithms Homework
type: hacks
courses: { compsci: {week: 6} }
categories: [C1.4]
---

class Student:
    def __init__(self, name, score):
        self.name = name
        self.score = score

    def __repr__(self):
        return f'{self.name}: {self.score}'

def bubble_sort_students(students):
    n = len(students)
    for i in range(n):
        for j in range(0, n - i - 1):
            if students[j].score > students[j + 1].score:
                students[j], students[j + 1] = students[j + 1], students[j]

# Sample student records
students = [
    Student("Alice", 85),
    Student("Bob", 70),
    Student("Charlie", 95),
    Student("David", 60),
    Student("Eva", 78)
]

# Sort the list of students based on their scores using bubble sort
bubble_sort_students(students)

# Print the sorted list of students
print("Sorted Student Records:")
for student in students:
    print(student)
