# Why DevOps?

Although, the software quality was improved using [SDLC](https://github.com/gul-ahmed/devops/blob/7c4d684edbeb15390a0c24a5e877b4d281a84f2a/1-SDLC/sdlc.md). We still had a lack of efficiency among the development team. 

- A typical software development team consists of Developers and Operations employees. Let us understand their job roles.
- A developer's job is to develop applications and pass his code to the operations team.
- The operations team job is to test the code, and provide feedback to developers in case of bugs. If all goes well, the operations team uploads the code to the build servers.
- The developer used to run the code on his system, and then forward it to operations team.
- The operations when tried to run the code on their system, it did not run!
- But, the code runs fine on the developer's system and hence he says “It is not my fault!”
- The operations then marked this code as faulty, and used to forward this feedback to the developer.
- This led to a lot of back and forth between the developer and the operations team, hence impacted efficiency.
- This problem was solved using Devops!

# What is DevOps?

Devops is a software development methodology which improves the collaboration between developers and operations team using various automation tools. These automation tools are implemented using various stages which are a part of the Devops Lifecycle.

<br>

![devops](https://github.com/gul-ahmed/devops/blob/38c0c3d5fc7dd7aaf2e4c6285bc814cff87e0a2c/images/devops.png)


# How DevOps Works?

Under a DevOps model, development and operations teams are no longer “siloed.” Sometimes, these two teams are merged into a single team where the engineers work across the entire application lifecycle, from development and test to deployment to operations, and develop a range of skills not limited to a single function.

DevOps teams use tools to automate and accelerate processes, which helps to increase reliability. A DevOps toolchain helps teams tackle important DevOps fundamentals including continuous integration, continuous delivery, automation, and collaboration.

# The DevOps lifecycle

The DevOps Lifecycle divides the SDLC lifecycle into the following stages:

![do_sdlc](https://github.com/gul-ahmed/devops/blob/43a7fcd40c464538eb88a1da21e026ce357cdf26/images/do_lifecycle.png)

![](https://github.com/gul-ahmed/devops/blob/43a7fcd40c464538eb88a1da21e026ce357cdf26/images/How-DeveOps-Works.png)


| Stage                 | Description                                                                                                                                                                                                                                                   |
|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Continuous Development** | Involves committing code to version control tools **`(e.g., Git, SVN)`** for version management. Utilizes build tools **`(e.g., Ant, Maven, Gradle)`** to package code into an executable file, ready for testing by Quality Assurance (QA) teams.                                   |
| **Continuous Integration**  | A critical point in the DevOps lifecycle, this stage focuses on integrating different stages of the process. It is key to automating the entire DevOps process, ensuring seamless collaboration and synchronization.                                                  |
| **Continuous Deployment**  | Code is built, the application or environment is containerized, and the result is pushed to the desired server. Key processes include Configuration Management, Virtualization, and Containerization, enabling efficient deployment.                                |
| **Continuous Testing**     | Involves automated testing of applications pushed by developers. If errors occur, the integration tool sends a message notifying developers. Successful tests trigger a message to the Integration tool, pushing the build to the production server.              |
| **Continuous Monitoring**   | This stage continuously monitors deployed applications for bugs or crashes. Additionally, it can collect user feedback. The gathered data is sent to developers to make improvements to the application.  |

# Devops Tools

Above discussed Devops Methodology cannot be put into action without it’s corresponding tools. Lets discuss the devops tools with their respective lifecycle stages.

![devops-tools](https://github.com/gul-ahmed/devops/blob/0670eae538eb5da0b387978feba2c1fa06993679/images/devops-tools.png)

**1. Continuous Development**

- This phase includes **planning** and **coding** the software's functions. While there are no specific tools for planning, various tools are available for code maintenance.
- During the planning phase, the project's vision is set, and then in the coding phase, they actually start writing the code.
- You can write the code in any language, but to keep it organized and work together smoothly, we use tools called Version Control. These tools are part of Continuous Development in DevOps. The most well-known ones include **Git, SVN, Mercurial, CVS, and JIRA.**

**2. Continuous Testing**

- After creating the code, it's not a good idea to release it right away. We should first test it for bugs and make sure it performs well.
- Using manual testing is not very efficient. Hence we use **Automated testing!**
- We use tools like **Selenium, TestNG, JUnit, or NUnit** to make our tests run automatically.
- Automated testing is great because it saves a bunch of time and effort compared to manual testing. In addition, creating reports is a big advantage. It makes it much easier to figure out which test cases didn't work in a group of tests. You can also scheduled these tests to run automatically at planned times. 

**3. Continuous Integration**

- The stage is a critical point in the whole Devops Lifecycle. It deals with integrating the different stages of the devops lifecycle, and is therefore the key in automating the whole Devops Process.
- This DevOps phase is super smart. It might not seem important in the first release, but as you go on, you'll see how crucial it is.
- Continuous Integration (CI) is a big deal even in the first release. It's super helpful to connect CI tools with configuration management tools for deployment.
- Without a doubt, the most well-known CI tool out there is **Jenkins**. Other popular CI tools include **Bamboo** and **Hudson**.
- CI tools are like conductors that make other DevOps tools work together smoothly. Whether it's tools for Continuous Development, Continuous Testing, Continuous Deployment, or Continuous Monitoring, CI tools can be connected with all of them.
- When Jenkins is connected with Git or SVN, it can automatically set up tasks like fetching code from shared repositories. It gets that code ready for builds and testing. Jenkins can build these tasks at planned times during the day or whenever new code is pushed to the central repository.
- When we integrate Jenkins with testing tools like Selenium, we make Continuous Testing happen. First, we build the code using tools like Maven, Ant, or Gradle. Once the code is built, Selenium steps in to automatically run the code. How does it do that? By making a set of test cases and running them one by one. The role of Jenkins/Hudson/Bamboo here would be to schedule/automate “Selenium to automate test case execution”.
- When integrated with Continuous Deployment tools, Jenkins/Hudson/Bamboo can trigger the deployments, planned by configuration management/containerization tools.
- And finally, Jenkins/Hudson can be integrated with monitoring tools like Splunk/ ELK/ Nagios/ NewRelic, to continuously monitor the status & performance of the server where the deployments have been made.

**4. Continuous Deployment**

- This (Continuous Deployment) is the phase where the action actually happens.
- In this stage the code is built, the environment or the application is containerized and is pushed on to the desired server. The key processes in this stage are Configuration Management, Virtualization and Containerization.
- DevOps wouldn't be complete without Configuration Management tools or Containerization tools. These tools are crucial for making Continuous Deployment (CD) possible.

  **`1. Configuration Management Tools`**
  - Configuration Management is the act of establishing and maintaining consistency in an applications’ functional requirements and performance. In simpler words, it is the act of releasing deployments to servers, scheduling updates on all servers and most importantly keeping the configurations consistent across all the servers.
  - For this, we have tools like **Ansible, Puppet, Chef, SaltStack** and more.
 
  **`2. Containerization Tools`**
  - Containerization tools are other sets of tools that help in maintaining consistency across the environments where the application is developed, tested and deployed. It eliminates any chance of errors/failure in the production environment by packaging and replicating the same dependencies and packages used in the development/testing/staging environment.
  - The clear winner here is **Docker**, which was among the first containerization tool ever. Earlier, this act of maintaining consistency in environments was a challenge because VMs and servers were used, and their environments would have to be managed manually to achieve consistency. Docker containers threw this challenge up above and blew it out of the water.

**5. Continuous Monitoring**

- Continuous Monitoring is like keeping an eye on how well your application is doing. Just developing and launching it isn't enough; we need to watch its performance.
- Monitoring is crucial because sometimes bugs can sneak through testing, and we want to catch and fix them quickly.
- The stage continuously monitors the deployed application for bugs or crashes. It can also be setup to collect user feedback. The collected data is then sent to the developers to improve the application.
- **Splunk, ELK Stack, Nagios, Sensu, NewRelic** are some of the popular tools for monitoring. When used in combination with Jenkins, we achieve Continuous Monitoring.
- To minimize the consequences of buggy features, monitoring is a big add-on. Buggy features most often tend to cause financial loss. So, all the more reason to perform continuous monitoring.
- Monitoring tools also report failure/ unfavorable conditions before your clients/ customers get to experience the faulty features. Don’t we all prefer this?
