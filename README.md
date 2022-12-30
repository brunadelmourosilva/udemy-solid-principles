# SOLID Principles: Introducing Software Architecture & Design

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

To solve this problem, we can create an interface and the same will be implemented for the classes. After, this interface will be passed in the constructor parameter, avoiding overloaded methods.

![image](https://user-images.githubusercontent.com/61791877/210023183-f172a5fe-c682-4e65-90aa-2d2851e2fb7e.png)

### Key Takeways

![image](https://user-images.githubusercontent.com/61791877/210023543-18b34cfc-c70a-42b9-9f68-9f1ce833f5be.png)

![image](https://user-images.githubusercontent.com/61791877/210023562-33036087-2f5e-4aba-a110-71622eae371e.png)

### Wrap up

![image](https://user-images.githubusercontent.com/61791877/210023853-5b7171de-c227-4c5d-a70b-1c6b99f77141.png)


---


