# Ex.No.6 – AI-Assisted Programming and Debugging

Date: 07-11-2026
Register No: 212225040003

## Aim

To write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights using multiple AI tools.

## AI Tools Required

1. ChatGPT
2. Google Gemini
3. GitHub Copilot
4. Python
5. C
6. Java
7. Visual Studio Code

## Explanation

In this experiment, I act as a software programmer and develop a Student Database Management System using multiple AI tools.

AI tools such as ChatGPT, Google Gemini and GitHub Copilot are used to generate programming code in Python, C and Java.

The generated codes are compared and analysed based on accuracy, readability, efficiency and code quality. Bugs are identified and corrected, code is optimized, time and space complexity are explained, and unit test cases are generated.

Python is also used to interact with AI APIs, compare the generated responses and retrieve sample data from a REST API.

## Procedure

### 1. Define the Scenario and Use Case

Scenario: Student Database Management System

A college needs a simple application to store and manage student information. The system helps users add, display and search student records.

The system can:

- Add student details.
- Display student records.
- Search students using register numbers.
- Identify invalid or duplicate records.
- Retrieve sample information using APIs.

Main Objectives

1. Generate code using Python, C and Java.
2. Compare outputs from different AI tools.
3. Identify and correct bugs.
4. Optimize the generated programs.
5. Explain time and space complexity.
6. Generate unit tests.
7. Compare manual coding with AI-assisted coding.

Figure 1: Student Database Management System

[Digitalization of Education Sector Is Boosting Student Information System](https://images.openai.com/static-rsc-4/o_VE2P6x7aI7wxLQp1UV9fA75hcRNLMZprTaM_NEovEMUuqScL8ktLmK-EvTTwzOnEug9JRSEM6MbYwHbmu9og7LE_JAqN6AP16wUP0FQjkOAuMI7L-uFT-I65IzS2ebkUQW7qBTmNF0KgSLbXnKlooJ6cDZfKU7TCZANwd5510?purpose=inline)

[linkedin.com](https://www.linkedin.com/pulse/digitalization-education-sector-boosting-student-cgshe?utm_source=chatgpt.com)

Illustration of a computer-based student record management application.

### 2. Identify Multiple AI Tools

ChatGPT: Used to generate programming code, explain algorithms and identify errors.

Google Gemini: Used to generate alternative programs and suggest code improvements.

GitHub Copilot: Used to provide code suggestions, debugging assistance and programming support in Visual Studio Code.

AI Tool Workflow

## Multiple AI Tools Workflow

ChatGPT

Code generation

Gemini

Code optimization

Copilot

Code assistance

Python Orchestration Program

Connects AI tools and compares responses

Code Analysis and Testing

Bug detection, optimization and unit tests

### 3. Generate Prompts Using AI Tools

Prompt 1 – Code Generation

"Act as an experienced software programmer. Develop a Student Database Management System using Python, C and Java. The program should add student details, display student records and search students using register numbers. Generate simple, readable and error-free code."

Prompt 2 – Bug Identification

"Act as a software debugging expert. Analyse the generated Python, C and Java programs. Identify syntax errors, logical errors and runtime errors. Explain the bugs and provide corrected code."

Prompt 3 – Code Optimization

"Act as a code optimization expert. Optimize the generated programs by improving readability, reducing unnecessary operations and handling errors properly. Explain the time and space complexity."

Prompt 4 – Unit Test Generation

"Act as a software testing engineer. Generate unit test cases for the Student Database Management System. Include valid input, invalid input, duplicate register numbers and student search tests. Provide expected outputs."

### 4. Generate Python Code Using AI

Python Program – Student Database Management System

```
students = []def add_student(name, reg_no):    for student in students:        if student["reg_no"] == reg_no:            print("Register number already exists")            return    students.append({        "name": name,        "reg_no": reg_no    })    print("Student added successfully")def display_students():    if not students:        print("No records found")        return    for student in students:        print(student)def search_student(reg_no):    for student in students:        if student["reg_no"] == reg_no:            print("Student found:", student)            return    print("Student not found")add_student("Aancy", "101")add_student("Aisha", "102")display_students()search_student("101")
```

Output

```
Student added successfully
Student added successfully

{'name': 'Aancy', 'reg_no': '101'}
{'name': 'Aisha', 'reg_no': '102'}

Student found: {'name': 'Aancy',
                'reg_no': '101'}
```

Figure 2: Python Programming

[Lecture 3 - CS50's Computer Science for Business](https://images.openai.com/static-rsc-4/8uj821ueLkpIeFTcs31KjMtVUROd4ln1TgyGDyWxK6mM6XCgt38jBCobrivDf8bcTBo3vmxqrPIsElsxQHkRSmA3LXTmd56U6-WOyh4bKl_waAlwNZdnzXy6kbmlefljU5tgv7RElWyzNPIcQqN1j9gle8eLt1iFCJXHSvGLIvE?purpose=inline)

[cs50.harvard.edu](https://cs50.harvard.edu/business/notes/3/?utm_source=chatgpt.com)

Python is used to implement the student record operations.

### 5. Generate C Code Using AI

C Program – Student Database Management System

```
#include <stdio.h>

struct Student {
    char name[50];
    int reg_no;
};

int main() {
    struct Student s[10];
    int n, i, search, found = 0;

    printf("Enter number of students: ");
    scanf("%d", &n);

    if (n < 1 || n > 10) {
        printf("Invalid number of students");
        return 0;
    }

    for (i = 0; i < n; i++) {
        printf("Enter name: ");
        scanf("%49s", s[i].name);

        printf("Enter register number: ");
        scanf("%d", &s[i].reg_no);
    }

    printf("Enter register number to search: ");
    scanf("%d", &search);

    for (i = 0; i < n; i++) {
        if (s[i].reg_no == search) {
            printf("Student found: %s\n",
                   s[i].name);
            found = 1;
            break;
        }
    }

    if (!found) {
        printf("Student not found");
    }

    return 0;
}
```

Output

```
Enter number of students: 2

Enter name: Aancy
Enter register number: 101

Enter name: Aisha
Enter register number: 102

Enter register number to search: 101

Student found: Aancy
```

Figure 3: C Programming

[Dracula Redefined - Visual Studio Marketplace](https://images.openai.com/static-rsc-4/e9HGmRg2mxV_bURxF43ZTLeZqpAc18dF2WJZf9ZtYL8MZlBhTU4Yk_679MfDFdHHSr1xJIqqxzYG_MeraYNnV1vMPNTngNhYzTgDbdZu8Bm5kypiQ3HQFCqZsxHZFSoThtb1kw_14wHb8rf9qphFGcpY0_SpGBAC_AvItvghpy0?purpose=inline)

[marketplace.visualstudio.com](https://marketplace.visualstudio.com/items?itemName=lakshits11.dracula-redefined\&utm_source=chatgpt.com)

C language uses structures and arrays to store and search student details.

### 6. Generate Java Code Using AI

Java Program – Student Database Management System

```
import java.util.Scanner;

class Student {
    String name;
    int regNo;

    Student(String name, int regNo) {
        this.name = name;
        this.regNo = regNo;
    }
}

public class StudentDatabase {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        Student[] s = new Student[10];

        System.out.print("Enter number of students: ");
        int n = sc.nextInt();

        if (n < 1 || n > 10) {
            System.out.println("Invalid input");
            sc.close();
            return;
        }

        for (int i = 0; i < n; i++) {

            System.out.print("Enter name: ");
            String name = sc.next();

            System.out.print("Enter register number: ");
            int reg = sc.nextInt();

            s[i] = new Student(name, reg);
        }

        System.out.print("Enter register number to search: ");
        int search = sc.nextInt();

        boolean found = false;

        for (int i = 0; i < n; i++) {

            if (s[i].regNo == search) {
                System.out.println(
                    "Student found: " + s[i].name
                );

                found = true;
                break;
            }
        }

        if (!found) {
            System.out.println("Student not found");
        }

        sc.close();
    }
}
```

Output

```
Enter number of students: 2

Enter name: Aancy
Enter register number: 101

Enter name: Aisha
Enter register number: 102

Enter register number to search: 101

Student found: Aancy
```

Figure 4: Java Programming

[New UI | IntelliJ IDEA Documentation](https://images.openai.com/static-rsc-4/L1Iat5sbaUmBrqf8c79N9KJrKWAXBfu3Hz1DSFd2WUkNtJU8tlNRNLj6Dbjt5Unac_rQQAlhuo1m4MCnCTPA8SxyLqWFgBRo-aOp8BUPdPxpqIdGwqXVSkTfOiCF_hZNDUjVc7eqSqz-yRDwF4rCOF3iYE7KMecsstcZIVSgqnU?purpose=inline)

[jetbrains.com](https://www.jetbrains.com/help/idea/new-ui.html?utm_source=chatgpt.com)

Java uses classes and objects to manage student records.

### 7. Integrate Python with Multiple AI APIs

Python is used as the main integration program to connect ChatGPT and Google Gemini through their APIs. The same prompt is sent to both tools, and their generated responses are compared.

Install the required libraries

```
pip install openai google-genai requests
```

Python API Integration Code

```
import osimport requestsfrom openai import OpenAIfrom google import genai# Read API keysopenai_key = os.getenv("OPENAI_API_KEY")gemini_key = os.getenv("GEMINI_API_KEY")if not openai_key or not gemini_key:    raise ValueError("API keys are missing")# Connect to ChatGPTopenai_client = OpenAI(api_key=openai_key)# Connect to Geminigemini_client = genai.Client(api_key=gemini_key)# Common promptprompt = """Act as a software programmer.Generate a Student Database Management Systemusing Python, C and Java.Include add, display and search operations."""# ChatGPT responsechat_response = openai_client.responses.create(    model="gpt-5.5",    input=prompt)chat_output = chat_response.output_text# Gemini responsegemini_response = gemini_client.models.generate_content(
```

The OpenAI Responses API and Google Gen AI Python SDK are used for the two model requests.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://developers.openai.com\&sz=32)

OpenAI API Reference+1



Output Format

```
CHATGPT OUTPUT
[Generated program]

GEMINI OUTPUT
[Generated program]

OUTPUT COMPARISON
ChatGPT characters: [Actual count]
Gemini characters: [Actual count]

API DATA
1 Leanne Graham ...
2 Ervin Howell ...
3 Clementine Bauch ...

API integration completed successfully
```

Note: The actual responses and character counts are generated when the program is executed with valid API keys. JSONPlaceholder provides demonstration user information, not actual college student records.

Figure 5: API Integration

[GraphQL vs. REST: Exploring how they work | Contentful](https://images.openai.com/static-rsc-4/w5zYGV1nB-8TTATmFPQA3Hl8hcIDQkwxngVU8bgB63AoR1MDAQY5DQagWabV188pzpRjj_hRKKjzf3JbVuVqEIIFR0zycCXunYxVPhWTBCxwNjO2mvUsbQ-7FCR7lQw4V28_30wXmfIfoIIwMvDuu-WZQt4xgmdWT_BxlWZcJMU?purpose=inline)

[contentful.com](https://www.contentful.com/blog/graphql-vs-rest-exploring-how-they-work/?utm_source=chatgpt.com)

Python sends API requests and receives data in JSON format.

### 8. Compare AI-Generated Outputs

The same prompt is provided to ChatGPT and Gemini. Their generated programs are compared using the following criteria.

| Criteria       | ChatGPT            | Gemini             |
| -------------- | ------------------ | ------------------ |
| Python code    | Check readability  | Check readability  |
| C code         | Check correctness  | Check correctness  |
| Java code      | Check structure    | Check structure    |
| Error handling | Examine exceptions | Examine exceptions |
| Optimization   | Examine efficiency | Examine efficiency |
| Explanation    | Check clarity      | Check clarity      |

Analysis

Both AI tools can generate programs for the same application. Their outputs may differ in coding style, structure and explanation. The generated programs must be executed and verified to identify the better solution.

### 9. Identify Bugs and Optimize Code

Bug Identification

Incorrect code:

```
def search_student(reg_no):    for student in students:        if student["reg_no"] == reg_no:            print("Student found")        else:            print("Student not found")
```

Bug: The program prints "Student not found" for every record that does not match, even when the required student exists later in the list.

Corrected Code

```
def search_student(reg_no):    for student in students:        if student["reg_no"] == reg_no:            print("Student found")            return    print("Student not found")
```

Code Optimization

A dictionary can be used to improve searching performance.

```
students = {    "101": "Aancy",    "102": "Aisha"}def add_student(reg_no, name):    if reg_no in students:        print("Register number already exists")    else:        students[reg_no] = name        print("Student added successfully")def search_student(reg_no):    print(students.get(reg_no, "Student not found"))add_student("103", "Ravi")search_student("101")
```

Output

```
Student added successfully
Aancy
```

Figure 6: Bug Identification and Optimization

Before correction

Unnecessary repeated searching and incorrect output.

After correction

Correct search result and improved lookup using a dictionary.

### 10. Explain Time and Space Complexity

Complexity analysis is used to measure the efficiency of the generated programs.

| Operation                               | Time Complexity | Space Complexity |
| --------------------------------------- | --------------- | ---------------- |
| Add student (list with duplicate check) | O(n)            | O(1) additional  |
| Display students                        | O(n)            | O(1) additional  |
| Search student (list)                   | O(n)            | O(1) additional  |
| Search student (dictionary)             | O(1) average    | O(1) additional  |
| Store student records                   | —               | O(n)             |

Explanation

- O(1) represents constant time.
- O(n) represents linear time.
- O(n) storage means memory increases according to the number of student records.
- Dictionary searching takes O(1) average time.

### 11. Generate Unit Tests

Unit testing is used to verify whether individual functions work correctly.

Python Unit Test Code

```
import unittestdef find_student(students, reg_no):    for student in students:        if student["reg_no"] == reg_no:            return student    return Noneclass TestStudentDatabase(unittest.TestCase):    def setUp(self):        self.students = [            {"name": "Aancy", "reg_no": "101"},            {"name": "Aisha", "reg_no": "102"}        ]    def test_valid_search(self):        result = find_student(self.students, "101")        self.assertEqual(result["name"], "Aancy")    def test_invalid_search(self):        result = find_student(self.students, "999")        self.assertIsNone(result)    def test_empty_database(self):        result = find_student([], "101")        self.assertIsNone(result)if __name__ == "__main__":    unittest.main()
```

Output

```
test_valid_search ... ok
test_invalid_search ... ok
test_empty_database ... ok

Ran 3 tests

OK
```

Figure 7: Unit Testing

[Task 7: Running the Auto-grading Tests :: Introduction to Web Dev](https://images.openai.com/static-rsc-4/PFDNdsPEstTYd8J7PqEYpg8xvU7tO_zjFz1-hSnV4dNGCT-e-LqF2AJ76ysMwN05SgNA_4IgNbYBL91xsd25zrNEhnviATij35rhX3zhwS6guoCcEWqPKH6zDWZtk-QZI-ugXwVQFHYw2mgkoY81zZ6vhCSpLv_bSkxG5S_oW2Q?purpose=inline)

[education.launchcode.org](https://education.launchcode.org/intro-to-web-dev-curriculum/assignments/orbit-report/testing/index.html?utm_source=chatgpt.com)

Expected result: 3 tests passed

### 12. Compare Manual Coding Versus AI-Assisted Coding

| Aspect            | Manual Coding          | AI-Assisted Coding       |
| ----------------- | ---------------------- | ------------------------ |
| Code generation   | More time required     | Faster generation        |
| Debugging         | Manual identification  | AI suggestions           |
| Code optimization | Programmer performs it | AI suggests improvements |
| Error handling    | Requires experience    | AI provides suggestions  |
| Learning          | Requires practice      | Provides explanations    |
| Accuracy          | Depends on programmer  | Requires verification    |

Discussion

Manual coding improves programming knowledge and problem-solving skills. AI-assisted coding reduces development time and provides suggestions for debugging and optimization. However, the generated code must be checked and tested before implementation.

Figure 8: Manual Coding vs AI-Assisted Coding

Manual Coding

Write, debug and optimize code manually.

AI-Assisted Coding

Generate code and receive debugging suggestions.

### 13. Code Quality Analysis

The generated programs are evaluated based on the following criteria.

| Criteria        | Description                    |
| --------------- | ------------------------------ |
| Accuracy        | Correctness of program output  |
| Readability     | Easy to understand             |
| Efficiency      | Minimum unnecessary operations |
| Error Handling  | Handles invalid inputs         |
| Maintainability | Easy to modify                 |
| Testing         | Passes unit test cases         |

Analysis

1. Python provides simple syntax and easy implementation.
2. C provides structured programming and efficient execution.
3. Java supports object-oriented programming.
4. ChatGPT and Gemini generate alternative programming solutions.
5. GitHub Copilot provides coding suggestions.
6. Unit testing helps identify errors and verify correctness.

### 14. Evaluation Method – Rubrics

The AI-generated programs are evaluated using the following rubric.

| Criteria        | Excellent (5)   | Good (4)        | Average (3)        | Poor (2)    |
| --------------- | --------------- | --------------- | ------------------ | ----------- |
| Accuracy        | Highly accurate | Mostly accurate | Some errors        | Many errors |
| Clarity         | Very clear      | Clear           | Moderate           | Confusing   |
| Technical Depth | Detailed        | Good detail     | Basic              | Limited     |
| Code Quality    | Well optimized  | Good structure  | Average            | Poor        |
| Relevance       | Fully relevant  | Mostly relevant | Partially relevant | Irrelevant  |

Rubric Evaluation Results

| AI Tool        | Accuracy | Clarity  | Code Quality |
| -------------- | -------- | -------- | ------------ |
| ChatGPT        | Evaluate | Evaluate | Evaluate     |
| Gemini         | Evaluate | Evaluate | Evaluate     |
| GitHub Copilot | Evaluate | Evaluate | Evaluate     |

## Conclusion

The experiment demonstrates how multiple AI tools can be used for code generation, debugging, optimization and software testing.

ChatGPT, Google Gemini and GitHub Copilot help programmers generate programs in Python, C and Java. Python is used to interact with AI APIs, compare generated responses and retrieve sample data through a REST API.

The experiment also explains bug identification, time complexity, space complexity and unit testing. AI-assisted programming improves development speed and provides useful suggestions, while manual verification is essential to ensure code correctness.

## Result

The corresponding prompt was used to generate and analyse programs using multiple AI tools. API interaction, code comparison, bug identification, optimization, complexity analysis and unit test generation were demonstrated.

Thus, the experiment on AI-Assisted Programming and Debugging was completed successfully.


