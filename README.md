# Architectural concepts
It's been a long time since the famous Model-View-Controller (MVC) pattern started to gain popularity in the software development industry and became one of the legends of the enterprise architecture design.

Basically, the model represents the knowledge that the view is responsible for presenting, while the controller mediates the relationship between model and view. However, these concepts are a little bit abstract, and this pattern may have different implementations depending on the language, platform, and purpose of the application. After a lot of discussions about which architectural pattern the framework follows, its authors declared that from now on, AngularJS would adopt Model-View-Whatever (MVW). Regardless of the name, the most important benefit is that the framework provides a clear separation of the concerns between the application layers, providing modularity, flexibility, and testability.

In terms of concepts, a typical AngularJS application consists primarily of a view, model, and controller, but there are other important components, such as services, directives, and filters.

The view, also called template, is entirely written in HTML, which provides a great opportunity to see web designers and JavaScript developers working side by side. It also takes advantage of the directives mechanism, which is a type of extension of the HTML vocabulary that brings the ability to perform programming language tasks such as iterating over an array or even evaluating an expression conditionally. Behind the view, there is the controller. At first, the controller contains all the business logic implementation used by the view. However, as the application grows, it becomes really important to perform some refactoring activities, such as moving the code from the controller to other components (for example, services) in order to keep the cohesion high.

The connection between the view and the controller is done by a shared object called scope. It is located between them and is used to exchange information related to the model.

The model is a simple Plain-Old-JavaScript-Object (POJO). It looks very clear and easy to understand, bringing simplicity to the development by not requiring any special syntax to be created.
