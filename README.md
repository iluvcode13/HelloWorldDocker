Docker is a platform that allows you to develop, ship, and run applications inside lightweight, portable containers. Containers package an application with all of its dependencies into a standardized unit for software development, ensuring that the application works seamlessly in any environment.

Key benefits of Docker:

Consistency: Runs the same across all environments (development, testing, production)

Isolation: Applications run in separate containers without interfering with each other

Portability: Can run on any machine that has Docker installed

Efficiency: Containers share the host OS kernel, making them much lighter than virtual machines

Scalability: Easy to scale applications up or down
Here’s a concise breakdown of the requirements into GitHub stories:

requirements
1. Set Up Java Environment
Ensure JDK 22/23 is installed and verify HelloWorld.java compiles locally. The app should print "Hello, Docker and Java!" when run.

2. Install and Configure Docker
Install Docker Desktop or CLI and confirm it works by running docker --version and the hello-world test container.

3. Create Dockerfile
Write a Dockerfile using openjdk:23 as the base image. Copy the compiled .class files, set WORKDIR, and define the CMD to run the Java app.

4. Build and Run the Container
Build the image with docker build -t hello-java . and run it. Verify the output matches the expected message.

5. Automate Compilation in Docker
Update the Dockerfile to compile the Java code inside the container instead of relying on local builds.

6. Fix Version Mismatch Errors
If encountering UnsupportedClassVersionError, align the JDK version in the Dockerfile with the host system (e.g., FROM openjdk:23).

7. Documentation & Submission
Write a README.md explaining Docker’s role, steps to reproduce, and include output screenshots. Push the code to GitHub and submit the repo link.
