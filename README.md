# Swift Project Setup for VS Code

## ✅ Check if Swift is Installed

1. Verify that Swift is installed on your system:
   ```bash
   swift --version

	2.	If not installed, download the latest version from Swift.org.

⸻

✅ Install Swift Extensions in VS Code

To enable Swift development in VS Code, install the following extensions:
	•	Swift for Visual Studio Code
	•	CodeLLDB (for debugging)

⸻

🛠️ Swift Project Setup

1️⃣ Navigate to Your Developer Folder

cd ~/Developer



⸻

2️⃣ Create a New Project Folder

mkdir MySwiftProject
cd MySwiftProject



⸻

3️⃣ Initialize a Swift Package

swift package init --type executable



⸻

4️⃣ Open the Project in VS Code

code .



⸻

5️⃣ Build and Run the Project

swift build
swift run



⸻

🐞 Debugging in VS Code (Optional)

To enable debugging, ensure CodeLLDB is installed and configure debugging in .vscode/launch.json:
	1.	Create a .vscode/launch.json file:

mkdir -p .vscode
touch .vscode/launch.json
open .vscode/launch.json


	2.	Add the following content:

{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Debug Swift",
            "type": "lldb",
            "request": "launch",
            "program": "${workspaceFolder}/.build/debug/MySwiftProject"
        }
    ]
}


	3.	Start debugging:
	•	Open Run and Debug in VS Code.
	•	Select Debug Swift.
	•	Press F5 to start debugging.

⸻

✍️ Adding a New Swift File (Optional)

To create additional Swift files inside your project:
	1.	Using the terminal:

touch Sources/MySwiftProject/newfile.swift


	2.	Using VS Code:
	•	Open Command Palette (Cmd + Shift + P).
	•	Select “Swift: Create New Swift File…”.
	•	Name your file and start coding.

⸻

🔄 Modify Code & Rebuild

After making changes to your Swift files, rebuild and run your project:

swift build
swift run



⸻

✅ You’re All Set! 🚀


