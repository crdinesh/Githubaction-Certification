# Githubaction-Certification

              #####################################Varibles and Secrets##################################################

              ## 1. Declaring variables at Each Step Level Username:dinesh --> Step $Username or "${{env.Username}}"
              ## 2. Declaring varaibles at job level --> can be accessible at all steps and to the sepcifc job
              ## 3. Declaring variables at WOrkflow level --> will be accessible for all jobs
              ##4. Reposioty level secrets --> <!--- ""${{secrets.password}} !>>> for variables ${{vars.userid}}
              ##5. wOrkflow dispatch --> event for manual entering values and run the pipeline manually
              ##6. Concurrency - RUn a single job at a time 
                 concurrency:
                   group: production-deployment
                   cancel-in-progress: true --> cancels the running job
                   cancel-in-progress: false --> will wait for the job to get finish

              ##7. timeout in minutes --> 
              ##8. Matrix strategy --> variations for each job