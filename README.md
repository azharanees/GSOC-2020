# Google Summer of Code 2020 - OWASP (Final Submission)

## Table of Contents

- [Overview](#overview)
    - [About me](#about-me)
    - [Project details](#project-details)
    - [Proposed summary](#proposed-summary)
    - [Work done](#work-done)

- [Contributions](#contributions)

- [Future work](#future-work)

- [Conclusion](#conclusion)

## Overview

### About Me

- **Name:** Azhar Ahamed
- **Major:** Computer Science
- **University:** University of Westminster
- **Institution:** Informatics Institute of Technology
- **GitHub:** [@azharanees](https://github.com/azharanees)
- **E-mail:** zhranees@live.com, azharanees1@gmail.com, azhar.2017815@iit.ac.lk
- **Telegram ID:** @azharanees
- **Project URL:** https://github.com/azharanees/OWASP-iGNITA<br>

### Project details

The OWASP Ignita consist of Static application security testing tool and Dashboard to view the results of the testing, Even Though there are many SAST tools available for testers, but the compatibility and the Environment setup process is complex. By using OWASP Ignita's Static Application Security Testing tool Testers will be able to analyse and review their code quality and vulnerabilities without any additional setup. OWASP IGNITA can be integrated in the DevSecOps toolchain to help developers to write and produce secure code.

Currently the following features are supported:



- [x] OWASP Top 10 vulnerabilities 
- [x] Static Application security Testing
- [x] Scanning Tools based on OWASP Top 10
- [x] Dashboard to view the results
- [x] Standalone JAVA Scanner
- [x] Maven plugin 




**Organisation:** OWASP Foundation<br>
**Project URL:** https://github.com/azharanees/OWASP-iGNITA<br>
**Mentor:** Spyros [(@northdpole)](https://github.com/northdpole), AZZEDDINE Ramrami [(@aramrami)](https://github.com/aramrami)<br>
**Proposal Title:** Building a Standalone Scanner for OWASP IGNITA to detect OWASP TOP 10 Vulnerabilities and building a plugin for IDE’s<br>
**Tag:** OWASP IGNITA<br>

### Proposed summary

**Proposed summary as per proposal**:

To overcome the problems related to complexity of sast tool setups, It is a fine game plan to build an own standalone analyser to detect vulnerabilities where the OWASP IGNITA will be independent from tools such as SonarQube, which will make the Framework more light and easy to set up, and users won’t be restricted to the API provided by the sonarqube or other scanners of such. Also creating a plugin for IDE’s which will be a faster way to detect vulnerabilities. And dockerize the Framework so the set up time will be minimal and less hectic. This plugin will also be proposed to be integrated into  DevSecOps toolchain; github/jenkins/owasp appsec pipelines. Additionally a developer guide will be written with guidelines, templates and other titles for future collaborators.

Requirement which satisfy the Important Selection Criteria,
- Vulnerabilities it can detect (out of the OWASP Top Ten?) - Focused on top Ten
- Can it be integrated into the developer's IDE? - Plugin is proposed to be developed
- How hard is it to set up/use? - Dockerizing for easy setup
- Can it be run continuously and automatically? - Will be tested and added to pipeline in github

### Work done

**Summary of the work done during the GSoC :**

Standalone Java scanner was developped to find and vulnerabilities on jar files which was built on top of spotbugs and findsecbug base. 

Spring boot api was developped integrating the standalone scanner which can be used to easily upload files to analyze.

Maven plugin was developped out of the standalone java scanner which can be integrated into other maven projects easily.

Integration of the scanner with the OWASP IGNITA dashboard to stage all the scanner results for better representation.

Dockerizing the scanner api and publishing it on [dockerhub]
(https://hub.docker.com/r/azhar1234/ignita-scanner-api)


    docker pull azhar1234/ignita-scanner-api

Code for the whole project can be found [here](https://github.com/azharanees/OWASP-iGNITA)

## Contributions

- [Network graph](https://github.com/azharanees/OWASP-iGNITA/network)
- [Contribution graph](https://github.com/azharanees/OWASP-iGNITA/graphs/contributors)


## Future Work

The followings are the projected milestone for next releases:

- Composing Docker images
- Improving the UI/UX of the dashboard
- Deploying the project into cloud so it will be available easy for access
- Making the scanner more flexible by adding a properties file which users can edit and set rules and analysis


## Conclusion

Working on this project was one of the best experience I got which made me learn many things technical and non-technical also helped my network to grow. My mentor was very supportive and almost everyday he was checking on me and provided me with resources that helped me successfully complete this project. GSoC helped me get started on contributing to the open source even though this year's GSoC period is coming to an end, Looking forward to work on open source projects and the OWASP organization.



