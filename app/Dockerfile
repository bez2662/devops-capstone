# Use Tomcat as the base image (it can run Java web apps)
FROM tomcat:9.0

# Remove default Tomcat apps
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy our built app into Tomcat
COPY target/devops-app.war /usr/local/tomcat/webapps/ROOT.war

# Expose port 8080
EXPOSE 8080

# Start Tomcat
CMD ["catalina.sh", "run"]
