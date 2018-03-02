# scimserver
SCIM Server aims at implementing SCIM specification. SCIM protocol is meant for safe and easy collection/distribution of User information based on standard guidelines defined by Specification and yet extensible. Below is the link to specification document.
https://tools.ietf.org/html/rfc7643

Below is the plan of implementation of server
1. Getting the REST APIs up with dummy data available for testing
2. Writing the connectors either part of this service or separate service which writes/updates/deletes data to AD/Other LDAPs/Database
   Priority order goes as: <br>
      a. Database <br>
      b. Active Directory (AD) <br>
      c. OUD (Oracle Universal Directory) <br>
   All above projects will most likely will be executed as separate libraries on their own so they could be useful to others. I will start with Oracle DB  and MySQL.
   All connectors will get REST APIs to configure Store details, Mappings between REST API attributes and Queries that we can fire against DB

Above Server should be suffice for other people to start building on this work. Since the project is distributible, I hope this project will grow bigger and will be helpful for other people to.
