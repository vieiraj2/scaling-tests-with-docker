# Scaling Tests with Docker
This repo is related to the [Scaling Tests with Docker] course from [Test Automation University].

There are two problems that every company faces with testing and development:

- One, higher-level tests, like Service and UI tests, can take a long time to run, especially in sequence.
- And two, variables outside of the test, like environments or services, can block development in its tracks, or worse, cause errors or failures in our tests that are difficult to debug and triage.

This is where Docker and containers come in to save the day!

Although C# with .NET Core is used in the Selenium examples, Docker is independent of the language and works for Windows, Mac, and Linux.

## NOTE: You must have .NET Core installed

Download the [.NET Core 2.1 SDK] and install it on your machine
- Click on .NET Core Installer for 2.1.X (latest 2.1)

## Running the tests

As of this writing, the easiest way is to run one of the following in the command line:

- `dotnet test --settings .runsettings --filter testcategory=standings`
    - Run tests based on category
    
- `dotnet test --settings .runsettings --filter name~lcs`
    - Run tests based on name
    
[Microsoft's documentation] on their `dotnet test` command can be found here: 

## Questions or Feedback

Many thanks to [Carlos Kidman], who provided this material for free learning.

- [LinkedIn]
- [Twitter]
- [YouTube]

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [Test Automation University]: <https://testautomationu.applitools.com>
   [Scaling Tests with Docker]: <https://testautomationu.applitools.com/scaling-tests-with-docker/>
   [Carlos Kidman]: <https://github.com/ElSnoMan>
   [Microsoft's documentation]: <https://docs.microsoft.com/en-us/dotnet/core/tools/dotnet-test?tabs=netcore21>
   [Linkedin]: <https://www.linkedin.com/in/carlos-kidman/>
   [Twitter]: <https://twitter.com/CarlosKidman>
   [YouTube]: <https://www.youtube.com/channel/UCNvYBOCETf7MByrYKDTU3fQ>
   [.NET Core 2.1 SDK]: <https://dotnet.microsoft.com/download/dotnet-core/2.1>