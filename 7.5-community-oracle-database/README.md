# Run build

`docker build -t <user>/sonarqube:7.5-community-oracle-database .`

# Run container
 `docker run --name sonarqube-oracle \`
    `-p 9000:9000 \`
    `-e sonar.jdbc.username=<username> \`
    `-e sonar.jdbc.password=<password> \`
    `-e sonar.jdbc.url=<url> \`
    `-e sonar.web.javaAdditionalOpts="-Duser.timezone=America/Sao_Paulo" \`
    `-e sonar.ce.javaAdditionalOpts="-Duser.timezone=America/Sao_Paulo" \`
    `<user>/sonarqube:7.5-community-oracle-database` 