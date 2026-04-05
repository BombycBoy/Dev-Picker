# 🎯 Dev Pick

![License](https://img.shields.io/badge/License-MIT-blue)
![Python](https://img.shields.io/badge/Python-3.11-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![GitHub Repo](https://img.shields.io/badge/GitHub-OpenSource-blue)

> Dev Pick is a Python program that helps developers **pick the best IDEs or code editors** for their programming language.  
> Stop wasting time searching — get tailored recommendations instantly! ⚡

---

## 🧩 Features

- 🔹 Select your programming language  
- 🔹 Get IDE & code editor recommendations  
- 🔹 Shows platform compatibility (Windows, Mac, Linux)  
- 🔹 Quick links to official IDE/download pages  
- 🔹 Easy to extend with new languages or editors  
- 🔹 Lightweight and fast — built entirely in Python  

---

## 💻 Supported Languages & Editors

| Language | Recommended IDEs / Editors | Platform |
|----------|----------------------------|----------|
| Python   | PyCharm, VS Code, Thonny   | Windows, Mac, Linux |
| Java     | IntelliJ IDEA, Eclipse     | Windows, Mac, Linux |
| C#       | Visual Studio, Rider       | Windows, Mac |
| Web Dev  | VS Code, Sublime, Atom     | Windows, Mac, Linux |
| C/C++    | CLion, Code::Blocks, VS Code | Windows, Mac, Linux |
| Go       | GoLand, VS Code            | Windows, Mac, Linux |
| Ruby     | RubyMine, VS Code          | Windows, Mac, Linux |

---

## 🛠️ How Dev Pick Works

Dev Pick is written in **Python** and uses a **simple dictionary-based mapping** of languages to recommended editors.  
The program logic:

1. Ask the user to enter a programming language.  
2. Look up the language in a dictionary of IDE/editor recommendations.  
3. Display a formatted list with platform info and official links.  
4. Optionally, suggest alternative editors for advanced users.  

Example Python snippet:

```python
# Example: Lookup dictionary
dev_tools = {
    "python": ["PyCharm", "VS Code", "Thonny"],
    "java": ["IntelliJ IDEA", "Eclipse"],
    "c#": ["Visual Studio", "Rider"]
}

language = input("Enter your programming language: ").lower()
if language in dev_tools:
    print(f"Recommended IDEs/Editors for {language.capitalize()}: {', '.join(dev_tools[language])}")
else:
    print("Language not found. Please try another!")