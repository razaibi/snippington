# snippington
Code snippets for VSCode.

#### VSCode Snippets

Visual Studio Code allows using shortcuts to generate code and setup cursor locations to navigate through the generated code.


#### Setup steps

You can setup snippets in VS Code with the following steps:

1. Navigate to top bar and click on Code. Then navigate to *Preferences*.

![Preferences](https://github.com/razaibi/snippington/raw/main/img/VSCode_Step_01.png)

2. Click on *Configure User Snippets*.

![Configure](https://github.com/razaibi/snippington/raw/main/img/VSCode_Step_02.png)

3. Create a new snippets file. Remember you do not need to create a new in case you want to append snippets to a new file.

![CreateSnippets](https://github.com/razaibi/snippington/raw/main/img/VSCode_Step_03.png)

4. You will be prompted to enter the name of the new snippets file. Enter the name of the new snippets file. A _.json.code-snippets_ may be a good format to work with. 

![SnippetsPrompt](https://github.com/razaibi/snippington/raw/main/img/VSCode_Step_04.png)

![EnterNewSnippet](https://github.com/razaibi/snippington/raw/main/img/VSCode_Step_05.png)

5. Once you create the new file, you copy the contents from the files listed in the folders in this repository (dotnet, go, etc).

Here is a sample snippet:

```json
{
    "Go Hello": {
        "scope": "go",
        "prefix": "go: hello",
        "body": [
            "package main\n",
            "import (",
            "\t\"fmt\"",
            ")\n",
            "func main(){",
            "\tfmt.Println(\"Hello ${1:World}!!!\")",
            "}",
        ],
        "description": "Hello World in Golang."
    }
}

```

#### Attribution

*[Go Basic Snippets](https://raw.githubusercontent.com/razaibi/snippington/main/go/basic/go_basic.json.code-snippets)* : based on [Go By Example](https://gobyexample.com/)