# 🎯 C# Variables & User Input Project

## Lesson Snapshot
Learn to store information in variables and create interactive programs that talk to users! (Ages 8-18)

## Folder & File Map
```
VariablesAndInput/
├── .git/
├── .gitignore
├── VariablesAndInput.csproj
└── Program.cs
```

## Step-by-Step Build Guide

### 1. Fork and Clone the Repository ✅
- **Where we're working**: Making your own copy of today's sta- **What to do**: Go to [https://github.com/PhillyCoderDojo/session2-variables](https://github.com/PhillyCoderDojo/CSharp-Lesson-Two/tree/main) → Click "Fork" → Open GitHub Desktop → Clone your fork to your computer
  rter project
- **Code snippet**: None
- **Why it matters**: You get your own playground to experiment in
- **Git command**: `git clone https://github.com/YOUR-USERNAME/session2-variables.git`
- **📸 SCREENSHOT**: *Fork button in top right, then GitHub Desktop clone dialog*

### 2. Open Project in Rider ✅
- **What to do**: Open Rider → File → Open → Navigate to your cloned folder → Select it → Click OK
- **Where we're working**: Loading your project into the coding tool
- **Code snippet**: None
- **Why it matters**: Time to start coding!
- **Git command**: None
- **📸 SCREENSHOT**: *Rider with project loaded in Solution Explorer*

### 3. Create Your First Variable 📦
- **What to do**: Open Program.cs and type these lines
- **Where we're working**: Program.cs file
- **Code snippet**:
```csharp
string myName = "Alex";
Console.WriteLine("Hello, " + myName);
```
- **Why it matters**: Variables are like boxes that hold information
- **Git command**: `git add . && git commit -m "Add first string variable"`
- **📸 SCREENSHOT**: *Code editor showing the variable declaration*

### 4. Add Number Variables 🔢
- **What to do**: Add these lines below your name code
- **Where we're working**: Program.cs file
- **Code snippet**:
```csharp
int myAge = 12;
double myHeight = 5.5;
Console.WriteLine($"I am {myAge} years old and {myHeight} feet tall");
```
- **Why it matters**: Different boxes (variables) hold different types of things
- **Git command**: `git add . && git commit -m "Add integer and double variables"`
- **📸 SCREENSHOT**: *Code showing all three variable types*

### 5. Get User Input 💬
- **What to do**: Replace your code with this interactive version
- **Where we're working**: Program.cs file
- **Code snippet**:
```csharp
Console.Write("What is your name? ");
string userName = Console.ReadLine();
Console.WriteLine($"Nice to meet you, {userName}!");
```
- **Why it matters**: Programs become fun when they respond to users
- **Git command**: `git add . && git commit -m "Add user input for name"`
- **📸 SCREENSHOT**: *Console showing the prompt and user typing*

### 6. Ask for Age 🎂
- **What to do**: Add this code to ask for the user's age
- **Where we're working**: Program.cs file (add after name code)
- **Code snippet**:
```csharp
Console.Write("How old are you? ");
string ageText = Console.ReadLine();
int userAge = int.Parse(ageText);
Console.WriteLine($"Wow! In 10 years you'll be {userAge + 10}!");
```
- **Why it matters**: Converting text to numbers lets us do math
- **Git command**: `git add . && git commit -m "Add age input with calculation"`
- **📸 SCREENSHOT**: *Console showing age calculation result*

### 7. Build Profile Questionnaire 📋
- **What to do**: Create a complete profile program
- **Where we're working**: Replace all code in Program.cs
- **Code snippet**:
```csharp
Console.WriteLine("=== Profile Builder ===");

Console.Write("Enter your name: ");
string name = Console.ReadLine();

Console.Write("Enter your age: ");
int age = int.Parse(Console.ReadLine());

Console.Write("Enter your favorite color: ");
string color = Console.ReadLine();

Console.Write("Do you like pizza? (yes/no): ");
bool likesPizza = Console.ReadLine().ToLower() == "yes";

Console.WriteLine("\n=== Your Profile ===");
Console.WriteLine($"Name: {name}");
Console.WriteLine($"Age: {age}");
Console.WriteLine($"Favorite Color: {color}");
Console.WriteLine($"Likes Pizza: {likesPizza}");
```
- **Why it matters**: Combining everything into a real program
- **Git command**: `git add . && git commit -m "Create complete profile questionnaire"`
- **📸 SCREENSHOT**: *Full program output with user responses*

### 8. Push Your Branch 🚀
- **What to do**: In GitHub Desktop → Click "Push origin" to upload your branch
- **Where we're working**: Sending your code to GitHub
- **Code snippet**: None
- **Why it matters**: Backs up your work and prepares for sharing
- **Git command**: `git push origin my-variables`
- **📸 SCREENSHOT**: *GitHub Desktop showing successful push*

## Run & Test ▶️
- Press Ctrl+F5 or click the green ▶️ button
- Answer all the questions when prompted
- **Common Error**: "Input string was not in a correct format" - happens when typing letters for age
- **Fix**: Make sure to type only numbers when asked for age

## Bonus Challenge 🔥
Create a Personal Calculator that asks for two numbers and shows all math operations!

**Hint**:
```csharp
Console.Write("First number: ");
double num1 = double.Parse(Console.ReadLine());
Console.Write("Second number: ");
double num2 = double.Parse(Console.ReadLine());
Console.WriteLine($"{num1} + {num2} = {num1 + num2}");
// Add subtraction, multiplication, division!
```

**Super Stretch**: Use `int.TryParse()` to handle bad input:
```csharp
if (int.TryParse(Console.ReadLine(), out int result))
{
    Console.WriteLine($"You entered: {result}");
}
else
{
    Console.WriteLine("That's not a number!");
}
```
