# AzureWorkshopExercise
Scaffolded  .NET 4.8 MVC application used for Azure Workshop exercise.

## Setup	
1. Clone this repository and open it using VS2017
2. Create and checkout a feature branch with your name, for example: `develop-IR` 
3. Push your branch to remote (you will need it later)

## Publish and deploy web app
1. Right click on the project `AzureWorkshopExercise`
2. Click publish and in the newly opened menu select App Service
3. Select Create New one and then (Create profile)
4. In the newly opened window we will create app service, app plan and resource group:
    - App name: enter your App service name, for example: `AzureWorkshopExercise-dev`
    - Subscription: select Visual Studio Professional subscription
    - Resource group: click on New and then enter something like: `AzureWorkshopExercise-RSG-Dev`
    - Hosting plan: click on New and then enter something like: `AzureWorkshopExercise-ASP-Dev`
    - Leave Applications insights to none and click create
    - Verify that your web app is deployed and published by opening the website URL. 
    - Optional: Navigate to your Azure portal and examine what you created via VS


## CI/CD
1. To setup CI/CD go to your resrouce group, open your app service resource
2. On the left sidebar menu open Azure deployment center
3. In the newly opened view, add the following parameters:
    - Source: `Github`
    - Organisation: `Comparis`
    - Repository: `AzureWorkshopExercise`
    - Branch: `develop-{YourBranchSufix}`
    - Workflow option: select the option to create workflow
    - Click save in the right upper corner
4. Step 2. should have created and committed Github Actions workflow for you
5. To verify that your automatic pipeline works, go to repository merge `update-hero-section` and push to remote repository
6. Verify and observe the progress [TODO]
