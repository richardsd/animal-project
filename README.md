# AnimalProject

## 🐾 Exercise Overview

Your task is to extend this Angular project by implementing two basic services to fetch cat and dog facts, and then creating a reusable component to display these facts. Make sure to structure the solution in a scalable and extensible way.

## ✅ Tasks

1. **Explore the Codebase**
   - Familiarize yourself with the general project structure.
   - Review the following services and models:
     - Services: [CatService](./src/app/services/cat.service.ts), [DogService](./src/app/services/dog.service.ts)
     - Models: [CatFact](./src/app/models/cat-fact.ts), [CatFactsResponse](./src/app/models/cat-facts-response.ts), [DogFact](./src/app/models/dog-fact.ts), [DogFactsResponse](./src/app/models/dog-facts-response.ts)

2. **Implement Animal Fact Service(s)**
   - Implement at least one of the animal fact services: [CatService](./src/app/services/cat.service.ts) or [DogService](./src/app/services/dog.service.ts) (preferable the `CatService`).
   - Ensure the service fetches facts from an appropriate API and returns them in the expected format.

3. **Create a Reusable Component**
   - Create a new `AnimalFactList` component in the directory:  
     `src/app/components/animal-fact-list`
   - This component should be capable of displaying a list of animal facts.
   - It should work with any fact-providing service (e.g., CatService, DogService).
   - **Important:** The component must remain decoupled from specific services to allow for future extensibility.

4. **Integrate the Component**
   - Use the `AnimalFactList` component to display the appropriate facts based on the selected toggle state (already present in the `AppComponent`).
   - You can use any suitable method to inject the right service—but using the **Strategy Design Pattern** is preferred.

5. **Write Unit Tests**
   - Add tests to verify the functionality of:
     - The `AnimalFactList` component
     - Any logic used to switch between services
     - Relevant services and models

## ⚙️ Requirements

Make sure you have the following installed:

- **Node.js** (v18 or higher)
- **npm** (v9 or higher)
- **Angular CLI** (v17.0.5)
- **Git** (to clone the repository)

## 🚀 Development

### Run the App

```bash
ng serve
```

Navigate to: [http://localhost:4200](http://localhost:4200). The application will automatically reload when you make changes.

### Generate Code

Use Angular CLI to generate components, services, pipes, directives and more:

```bash
ng generate component|directive|pipe|service|class|guard|interface|enum|module
```

### Run Tests

To execute the unit tests with [Karma](https://karma-runner.github.io):

```bash
ng test
```

## 📚 Resources

- [Angular CLI Documentation](https://angular.io/cli)
- [Angular Material - Button Toggle](https://material.angular.io/components/button-toggle/overview)
