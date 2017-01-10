# java-development-nuances

### typical flow
Request -> Serialize/Deserialize -> Controller -> Business Logic Layer -> DAO/DAOImpl -> DB

When accessing DB from an OOP language, typically need an ORM framework to do the conversion. For Java, there is Hibernate, JPA, and Hibernate with JPA.
* JPA -> both a specification and a bare bones implementation
 * reference: https://www.tutorialspoint.com/jpa/index.htm
* Hibernate -> standalone ORM framework that pre-dates JPA
 * uses EntityManager, JP-QL, Criteria Queries: https://docs.jboss.org/hibernate/entitymanager/3.5/reference/en/html/index.html
* Hibernate with JPA -> Hibernate but with JPA specs incorporated
 * uses SessionFactory, HQL, Criteria Queries (same name, diff implementation)
 * reference on what changed with JPA specs: http://stackoverflow.com/questions/20820880/hibernate-native-vs-hibernate-jpa

### links and resources
* https://www.reddit.com/r/java/comments/16ovek/understanding_when_to_use_jpa_vs_hibernate/
* http://softwareengineering.stackexchange.com/questions/211194/api-design-concrete-vs-abstract-approach-best-practices
* http://stackoverflow.com/questions/9881611/whats-the-difference-between-jpa-and-hibernate
