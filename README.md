# azure-devops-cli-howto

First install the following cli utility called az
 * https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest
 
Then install the extension for az called 'az-devops' found here:
 * https://github.com/Azure/azure-devops-cli-extension

If you work with multiple projects, or multiple organizations you will want to set these values as the one you most frequently use, you can override this by specifying the parameter in your indvidiual command

Next, configure your organization you plan to work with:
 * az devops configure --defaults organization=https://dev.azure.com/[OrganizationName]
 
Then configure your project you will work with
 * az devops configure --defaults project=[ProjectName]

then log into azure via cli with your credentails
 * az login
 
if you are using a PAT, then use
 * az devops login

finally you are able run devops commands in your workspace!
see the available commands here
 * https://docs.microsoft.com/en-us/cli/azure/ext/azure-devops/repos/pr?view=azure-cli-latest


