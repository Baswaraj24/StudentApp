# Use the official Tomcat image as the base image
FROM tomcat:latest

# Copy the WAR file into the Tomcat webapps directory
COPY target/studentapp-2.5.war /usr/local/tomcat/webapps/

# Copy the custom index.jsp file into the Tomcat webapps/ROOT directory
COPY WebContent/index.jsp /usr/local/tomcat/webapps/ROOT/

# Expose port 8080
EXPOSE 8080

# Start Tomcat when the container starts
CMD ["catalina.sh", "run"]
