# Jenkins:-
 ->Jenkins is an open-source automation platform that help Devops teams create and test s/w projects. It's used to  
    manage & control several stages of s/w delivery process.including:
                1.Build
                2.Documentation.
                3.Automated Testing.
                4.Packing.
                5.Static code analysis.
 ->Jenkins is written in java & has plugins designed for continous integration.It's used to implement CI/CD workflows,
     called"Pipeline". 

# Build:-
-> Build tools automate the creation of executable applications from source code.Building includes compiling,linking& 
    packaging the code into a usable or executable form.
->Jenkins supports several types of build jobs projects such as free style projects,pipelines,multi-configuration  
     projects,folders,multibranch pipelines & organization folders.

# Plugins:-
-> A Plugin is a s/w component that adds a specific feature to an existing computer program.
-> Plugins are the primary means of enhancing the functionality of a jenkins environment to suit   
    organization-or-user-specific needs
    *Build tools,Cloud Providers,Analysis tools*

# CI/CD:-
     The main concepts attributed to CI/CD are "continous integration,continous deelivery/depolyment". CI/CD
  is a method to frequently deliver apps to customers by introducing automation into the stages of app development.

# Pipelines:-
    It is a suite of plugins which supports implementing & intergrating continous delivery pipelines into jenkins.
    Pipelines are two types:
        1.Scripted.
        2.Declarative.

# Note:- 
 Jenkins is used by thousands of development teams other DevOps tools.include:
 Git,Docker,Cucumber,Ansible,Teamcity,Nagios............   

# Continuous Integration(CI):-
        CI is a Devops s/w development practice where developers regularly merge their code changes into a central
    repository,after which automated builds and tests are run.  
  ![Preview](image-1.png)

  # Version control system:-
         Version control also known as "Source control or revision control" is an important s/w development practice for 
    tracking & managing changes made to code & other files. It is closily related to source code management.     
  ![Preview](image-2.png)
Generation:
1.Single system version control
![preview](image-3.png)
2.Cliwnt server version control
![preview](image.png) 
       Centrolized version control system(CVCs) is a traditional version control system where the sourse code is stored
  in a central servce maintained by a single autority. Developers check out the code the need to work on & make changes directly to that codebase. Once the changes are made,they commit the code back to the centrol servce.  

  3.Distributed version control system(DVCs)
        Dvcs is a envolution of version control system that address the limitations of CVCs by allowing developers to 
    create local copies of the code repository,complete with the entire history each developer has a full copy of the repository on their local machine,including the changes history.     
        
  ## Terms:

  1.Repository:
      A repository is a data structure that stores metadata for a set of files or directory strucure.
    -> Source code repository: Git,GitHub,Apache subversion,chat GPT.
    -> Artifact repository: Stores build artifacts produced by continous integration & makes them available for
                             automated deployment to testing,staging &production environment.
                             ex:JFrog
  2. Artifact:
       An Artifact is an assemble of your project assets that you put together to test,deploy or disstribute your s/w
     solution or its part.
  3.Quality Gate:
        A Quality Gate is an enforced measure built into your pipeline that the s/w needs to meet before it can proceed to the next step.
    -> Rule:Quality Gate output a status(pass,warn,fail)

   Planning---->Design---->Development---->Deployment
           QG         QG               QG
   4.Promotion:

