# What I've Learned at the 16th lecture of 401 code...

## Many to many relationships

1. In order to map a many-to-many association, we use the @ManyToMany, @JoinTable and @JoinColumn annotations.

2. The @ManyToMany annotation is used in both classes to create the many-to-many relationship between the entities.

3. The @JoinColumn annotation is used to specify the join/linking column with the main table. Here, the join column is employee_id and project_id is the inverse join column since Project is on the inverse side of the relationship.

4. In the Project class, the mappedBy attribute is used in the @ManyToMany annotation to indicate that the employees collection is mapped by the projects collection of the owner side.

5. The Model Classes : The model classes Employee and Project need to be created with JPA annotations:


- Employee class

@Entity
@Table(name = "Employee")
public class Employee { 
    // ...
 
    @ManyToMany(cascade = { CascadeType.ALL })
    @JoinTable(
        name = "Employee_Project", 
        joinColumns = { @JoinColumn(name = "employee_id") }, 
        inverseJoinColumns = { @JoinColumn(name = "project_id") }
    )
    Set<Project> projects = new HashSet<>();
   
    // standard constructor/getters/setters
}

- Project class

@Entity
@Table(name = "Project")
public class Project {    
    // ...  
 
    @ManyToMany(mappedBy = "projects")
    private Set<Employee> employees = new HashSet<>();
    
    // standard constructors/getters/setters   
}


6. both the Employee class and Project classes refer to one another, which means that the association between them is bidirectional.




