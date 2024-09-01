# TddBddFrameworkWithFitnesse
I have created and setup Fitnesse Framework with Examples to get you up and running pretty quickly. I started this project 8 years ago and now have gotten a little time to update and to use as demo for others who are looking having their organization adopt automation.

Step-by-Step Guide: Cloning and Running the TddBddFrameworkWithFitnesse Project
1. Clone the Project
First, you'll need to clone the project repository to your local machine. Here’s how you can do it:

Open your terminal or command prompt.

Navigate to the directory where you want to clone the repository.

Run the following command:

git clone https://github.com/randi2160/TddBddFrameworkWithFitnesse.git

This will download the project files to your local machine.

2. Install Visual Studio Community Edition
To work with this project, you’ll need Visual Studio installed on your machine. Follow these steps:

Download Visual Studio Community Edition from here.
Install Visual Studio, ensuring that you include the .NET desktop development and ASP.NET and web development workloads during installation.
3. Open the Project in Visual Studio
Once you have Visual Studio installed:

Open Visual Studio.
Click on File > Open > Project/Solution.
Navigate to the directory where you cloned the project (TddBddFrameworkWithFitnesse).
Select the .sln file (solution file) and click Open.
Visual Studio will load the solution, allowing you to build and run the project.

4. Build and Run the Project
To build and run the project:

Press Ctrl + Shift + B to build the solution.
Ensure that the build is successful and there are no errors.


Go to the folder and execute runfitnesse.bat file to launch fitness

here is a sample of the info you need to put in fitnesse to launch get your dll and perform reflection on it

!|QaTip.Fitnesse.Demo.DoTestFixture|

!define COMMAND_PATTERN {%m -r fitnesse.fitserver.FitServer,FitSharp\fit.dll,FitSharp\fitLibrary.dll -c FitSharp\suite.config.xml %p}
!define TEST_RUNNER {Fitsharp\Runner.exe}
!path ..\FitnesseFramework\Fixtures\Fitnesse_Dlls\QaTip.Fitnesse.Demo.dll
!define TEST_RUNNER {Fitsharp\Runner.exe}

!contents -R2 -g -p -f -h  

We can test API, UI websrvice, database and anything that you need. If you can write code the skys the limit.

Explanation of the Provided Code
NavigateTo Method in DoTestFixture




