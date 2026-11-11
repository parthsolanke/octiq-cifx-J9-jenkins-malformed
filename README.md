# CI detection fixture

AC 5. A Jenkinsfile with no `pipeline {` / `node {` and no shell step - fails the readability gate. Must report UNREADABLE, must NOT fall through to 'no CI'.

Expected verdict line in the Octiq chat:

    Tests not run - CI config found (Jenkinsfile) but this detector could not read it
