## Spring guide: Accessing Data with JPA

### How are query methods defined when using Spring Data JPA?
I can't understand this , but it's like this
```public interface CrudRepository<T, ID extends Serializable>
  extends Repository<T, ID> {

    <S extends T> S save(S entity);

    T findOne(ID primaryKey);

    Iterable<T> findAll();

    Long count();

    void delete(T entity);

    boolean exists(ID primaryKey);
}
```
Notice the typical CRUD functionality:

save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
findOne(…) – get a single entity based on passed primary key value
findAll() – get an Iterable of all available entities in the database
count() – return the count of total entities in a table
delete(…) – delete an entity based on the passed object
exists(…) – verify if an entity exists based on the passed primary key value
This interface looks quite generic and simple, but actually, it provides all the basic query abstractions needed in an application.

### Which dependencies will you need in order to complete the Spring guide?
Spring Data JPA
H2 Database

### What annotations are used to specify an auto generated identification number for an Entity?
don't quote me ,I am guessing here 
@Entity
@Id
## Baeldung: Comparing repositories 

### Which of the Spring Data Repositories covered in the readings has the most methods available to it?
IDK

### Name a downstide of a Spring Data Repository.
it doesn't have the same level of maturity as other frameworks. For example, it doesn't offer much support for complex queries, so we have to write queries ourselves. Additionally, it doesn't support transactions, which can be a problem in some cases.
### How would you define an operation to find a student based on their name in a repo named StudentRepository which extends JpaRepository?

@Repository
public interface StudentRepository extends JpaRepository<Product, Long> {
    Student findByName(String studentName);
}
maybe ? 
