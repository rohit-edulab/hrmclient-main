# ReadMe file

Download file (clone the Repository):
```shell
git clone https://github.com/worldfellow/hrmclient.git
```
## Install npm packages

Install / Add the packages mentioned in the gitignore file :

### node modules: 
    ```shell
    npm install
    ```

### Environment files:
    * Create a folder for Environment in the src folder: src/environment
    * make the environment.prod.ts and environment.ts file
    * create an export variable with the structure of :
        
        `export const environment = {
            production: true,
            apiUrl: '',
            testUser: {
                token: {},
                email: '',
            },
            }; `
            for the prod file 
            and 
        `export const environment = {
            production: Boolean,
            _apiUrl: '',
            apiUrl: '',
            testUser: {
                tslint:disable
                token: {
                expires_in: Number,
                access_token: '',
                },
                tslint:enable
                email: 'user@user.user',
            },
        };` 
        for the environment file
