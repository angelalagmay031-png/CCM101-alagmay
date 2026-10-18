# Mission Reflection: Cloud Deployment Engineer

In this laboratory, I learned how Docker Compose can make cloud deployment easier and faster. Before doing this activity, I thought setting up a cloud application required many complicated steps and commands. However, I learned that using a configuration file can help organize the services and make the deployment process simpler.

**1. How does writing a docker-compose.yml file make a cloud engineer's job easier?**

Writing a `docker-compose.yml` file makes the work easier because all the settings for the application and database are written in one file. Instead of typing many commands separately, a cloud engineer can use `docker-compose up -d` to start the services. It also makes the deployment easier to repeat and manage.

**2. What happens if you make an indentation error in a YAML file?**

An indentation error can cause the YAML file to become invalid or make the configuration incorrect. YAML uses spaces to show the relationship between different settings, and it does not allow tabs for indentation. This taught me to be careful when writing and checking configuration files.

**3. Why did we use environment variables in the Compose file?**

We used environment variables to provide important configuration values, such as the database name, username, and password. These values help Nextcloud connect to MariaDB correctly. I also learned that real projects should protect sensitive information instead of putting passwords directly in configuration files.

**4. How did it feel to deploy Nextcloud in just a few minutes?**

I felt happy and excited because I was able to learn how a private cloud storage system can be deployed using containers. It was interesting to see how Nextcloud and MariaDB work together. The activity helped me understand that cloud technology can make deploying applications faster and more organized.

**5. How has your understanding of Cloud Computing evolved since Mission 1?**

Since Mission 1, my understanding of cloud computing has improved. I now understand that cloud computing involves more than accessing files online. It also includes managing servers, applications, networks, and databases. This laboratory helped me appreciate the importance of automation, proper configuration, and troubleshooting in cloud engineering.

Overall, this mission gave me more confidence in using Linux commands and Docker Compose. I learned that patience and attention to detail are important when deploying cloud applications.
