# Use official Tomcat image
FROM tomcat:9.0-jdk17-temurin

# Remove default ROOT app
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy WAR file into Tomcat
COPY target/service-registry-tms.war /usr/local/tomcat/webapps/service-registry-tms.war

# Expose port
EXPOSE 8080

# Start Tomcat
CMD ["catalina.sh", "run"]
