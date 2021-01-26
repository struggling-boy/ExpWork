https://cloud.tsinghua.edu.cn/f/c8880a9c30ab46f3b8df/

# Lab Doc for Interns

This document provides instructions for interns if they meet with any trouble.

## Project Assignment

Every intern joining our lab will have at least one Ph.D. or M.A. candidate (candidates in what follows) to work with. The project assigned to interns should be discussed with Prof. Zhao. Interns can also change candidates and projects but should let Prof. Zhao know.

Interns should provide their course schedules to candidates for bettering research task assignments.

### Task of Interns

Basically, it includes the following issues 

* **Literature survey and brainstorm**. Assist the candidate to investigate related works of the project and brainstorm which future work we can do.
* **Code Completion**. After get known of the project, candidates can offload some coding task or data preprocessing tasks to interns. If the task is too large, or there are any problems, interns should immediately contact candidates for help.

### Discussion

Interns can contact the corresponding candidates any time he/she meets with problems. Besides, regular meetings and discussions with the corresponding candidate are recommended. We recommend interns to wrap key points to be discussed in a simple PPT. The goal is to make the discussion to be more efficient than bare-talking. 

## Coding and Documenting

Most of the researches in our lab need coding to run simulations, numerical solution, and model training, etc. Considering the continuity of researches, interns have the responsibility to write code with explicit comments and related documents.

### Recommend IDE

We summarized useful IDE for different languages, and recommend interns to work with them if one does not know where to start.

|  Languages |                                                 IDE                                                 |
| :--------: | :-------------------------------------------------------------------------------------------------: |
|   Python   | VSCode (Development), PyCharm (Development), Spyder (Data Science), Jupyter Notebook(Data Science). |
|   MatLab   |                                        MatLab Editor, VSCode                                        |
| C, C++, C# |                                            Visual Studio                                            |

### Comments and Docstrings

Every code file should have detailed comments. Specifically,

* Every function should be explained by docstrings. The docstring style is not limited, but should contain the following elements (taking python file as an example):

  ```Python
  def foo(var1, var2):
      """
      <Descriptions to this function>
      
      Input:
      	var1 (Type of var1) : meaning of var1.
      	var2 (Type of var2) : meaning of var2.
      
      Output:
      	result (Type of result) : meaning of result.
      """
      pass

  ```

* Comments should be one-line-before or two-blank-after a statement, e.g.,

  ```python
  # var1 is for ...
  var1 = 2

  var2 = 10  # var2 is for

  ```

  We recommend interns to write comments at places where a new reader may not understand. When there are step by step statements, it is recommended to comments before each step, e.g.,

  ```python
  # Step 1. Intiate variables.
  var1 = 1
  var2 = 2

  # Step 2. Add two variables.
  var3 = var1 + var2

  ```

* (Not necessary, but recommend) At the beginning of a code file, the _author_, _date_, _function of the code_ should be provided.

### Documentation

When a project is finished (internship is over), we not only need to wrap results as papers, but also wrap up experiment codes, so that everyone can quickly know how to use the code, and the structure of code.

Generally, the documentation of code contains two parts:

* **Brief Introduction** of this repo and key idea. Note that the detailed description of the design of the algorithm, etc., should be included in papers rather than the documentation of the code repository.
* **Usage** shows how one can use the code, and run which code can achieve which goal.
* **The Structure of code** shows what contents each file (folder) contains.

### Git and GitHub Usage (Recommended)

Git is a version control tool that allows us to easily collaborate on coding. GitHub is more familiar to us, which is a platform to store code for exchange. We strongly recommend interns to use Git and GitHub when doing research. The [Git Guide](https://git-scm.com/docs/gittutorial) and [GitHub Guide](https://guides.github.com/activities/hello-world/) are perfect resources to get familiar with these tools.

## Computing Resource Usage

We have 3 servers so that interns can use to offload tasks. When interns need computing resource support, he/she can contact lyj18@mails.tsinghua.edu.cn to apply for a server account.

### Connect to Server

Basically, one can use _ssh_ command to connect to the server through cmd, PowerShell, terminal, etc. This requires interns to install ssh (openssh) first.

There are still some graphical softwares to achieve this. [MobaXTerm](https://mobaxterm.mobatek.net/) is a good choice.

If one prefers to totally graphical control of the server, he/she can use _remote desktop_ to connect to the server. To run remote desktop, one simply need to run "远程桌面连接" in windows.

### File Transferring

For single file transfer, [MobaXTerm](https://mobaxterm.mobatek.net/) is good enough. If one wants to transfer folders or numerous files between client and server, we recommend using _scp_ (which will also be installed with _ssh_) to achieve this.

### Modify Code on Server

One can modify code on the client-side. Then, transfer the modified code to the server through _scp_. A more convenient way is to use **VSCode** with plugin _Remote development_. This allows us to modify codes on the server in VSCode tab. In addition, one can even debug with it. A tutorial can be found in [VSCode Remote Tutorial](https://zhuanlan.zhihu.com/p/64849549).

### Running Code on Server

As suggested previously, one can either run code through:

* VSCode Remote. The code will not continue if you quit the connection.
* Remote Desktop controlling. The code will still run if you quit the connection.
* Running task in terminal through ssh. The code will stop if you quit the connection. One can use _tmux_ or _screen_ in this situation to avoid task dropping down.

## Paper Writing

We use [Overleaf](https://www.overleaf.com/) for paper writing collaboratively.

Enjoy doing research in our lab!
