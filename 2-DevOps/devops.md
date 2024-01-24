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

**Continuous Development**




