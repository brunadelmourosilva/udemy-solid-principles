# SOLID Principles: Introducing Software Architecture & Design ✅

## Single Responsability Principle

### Cohesion

Cohesion is the degree to which the various parts of a software are related.

__Higher cohesion__ helps attrain better adherence to the SRP. :heavy_check_mark:

![image](https://user-images.githubusercontent.com/61791877/209589716-bbfce202-0fc8-4af3-b12c-f35f24ef6f35.png)

>### Book: Desbravando SOLID

>To look for classes that are not very cohesive, we must to find classes like:

>- Have many different methods
>- Are changed frequently
>- Never stop growing
>- Have a many different imports classes

### Coupling

Coupling is defined as the level of inter dependency between various software components.

Aim for __lose coupling__. :heavy_check_mark:

![image](https://user-images.githubusercontent.com/61791877/209590216-99397905-47f4-478a-8e8c-a9262cda5834.png)

---

## Open Closed Principle

*"Software components should be closed for modification, but open for extension."*

![image](https://user-images.githubusercontent.com/61791877/210022721-499f28a6-6168-4610-ab35-42b53805b901.png)

### Example

This is a problem, because for each new feature, we would need to create a new overloaded method.

![image](https://user-images.githubusercontent.com/61791877/210023052-33c094fe-30cb-44aa-8f9f-d7f2c15a8310.png)

To solve this problem, we can create an interface and the same will be implemented for the classes. After, this interface will be passed in the constructor parameter(example: HomeInsuranceCustomerProfile), avoiding overloaded methods.

![image](https://user-images.githubusercontent.com/61791877/210023183-f172a5fe-c682-4e65-90aa-2d2851e2fb7e.png)

### Key Takeways

![image](https://user-images.githubusercontent.com/61791877/210023543-18b34cfc-c70a-42b9-9f68-9f1ce833f5be.png)

![image](https://user-images.githubusercontent.com/61791877/210023562-33036087-2f5e-4aba-a110-71622eae371e.png)

### Wrap up

![image](https://user-images.githubusercontent.com/61791877/210023853-5b7171de-c227-4c5d-a70b-1c6b99f77141.png)


---

## Liskov Substitution Principle

*"Object should be replacedable with their subtypes without affecting the correctness of the program."*

### The problem

![image](https://user-images.githubusercontent.com/61791877/211125093-6c9c942c-b656-4e4f-968c-3eafdeccbad6.png)

![image](https://user-images.githubusercontent.com/61791877/211125117-e082e1a5-706d-46f9-85b3-45625eefa9dc.png)

### The Solution 1

![image](https://user-images.githubusercontent.com/61791877/211125569-a681b040-8b99-4ebd-a52f-fab341860d75.png)

![image](https://user-images.githubusercontent.com/61791877/211125591-7efee452-f741-44ee-ac35-72dc980eff56.png)

### The problem

Here, we should deal with all Product objets, without make a typecast to identify the class that extends it.

![image](https://user-images.githubusercontent.com/61791877/211125844-3da24964-cf80-49a2-b56a-2d0f3a1de071.png)

### The Solution 2

![image](https://user-images.githubusercontent.com/61791877/211126733-fa4215ca-530f-446b-a423-34e8177418b4.png)

![image](https://user-images.githubusercontent.com/61791877/211126764-d4e052ef-d705-408d-8a23-849ba63a332b.png)

---

## Interface Segregation Principle

*"No client should be forced to depend on methods it does not use."*

### The problem

![image](https://user-images.githubusercontent.com/61791877/212438991-3af1621f-dd5a-477b-904b-98f11ea04314.png)

### The solution

![image](https://user-images.githubusercontent.com/61791877/212439334-31b09d55-3a94-412d-a2f7-ff03b8a8899b.png)

### Techniques to identify violations of ISP

![image](https://user-images.githubusercontent.com/61791877/212439707-02185b6c-291c-47f2-80cd-81a5d4f82ce6.png)

---

## Dependency Inversion Principle

*"High-level modules should not depend on low-level modules. Both should depend on abstractions."*

*"Abstractions should not depend on details. Details should depend on abstractions."*

### The problem

![image](https://user-images.githubusercontent.com/61791877/212784268-845e6146-9797-4d86-a1af-09c0366f4c48.png)


### The solution - Dependency inversion

![image](https://user-images.githubusercontent.com/61791877/212784301-b6726b71-2464-4307-9436-8677b98e4e79.png)

### Dependency injection

The injection will be made in the ProductCatalog through the constructor.

![image](https://user-images.githubusercontent.com/61791877/212784734-9da12014-06e0-4976-b8d0-d1988792dd00.png)

### Iversion of control

Insert the interface in the application and through the dependency injection, we can instantiate this implementation(under the table) without specify this what is the implementation.

Example: https://www.geeksforgeeks.org/spring-understanding-inversion-of-control-with-example/

![image](https://user-images.githubusercontent.com/61791877/212785599-a51ea803-c1f6-4f21-8397-86737630c02f.png)

