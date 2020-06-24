# Angular-CRUD-
Develped for performing crud operations using Angular

# Endpoint Client
### Create a New Branch

  - Click on Branches Button in VSCode on the bottom left corner
  - Select `Create New Branch From`
  - Enter New Branch Name
  - Select origin/master
  - Do a git pull origin master

### Before Deployment / For Testing

**on endpoint client:**
  - Make sure you are in your feature branch or enter the command `git checkout branch-name`
  - Enter the command `git pull origin master`
  - Resolve Merge Conflicts if any
  - Enter the command `yarn build`
  - Enter `git add .`
  - Enter `git commit -m ‘message’ `
  - Enter `git push`

- ### Dashboard Component
Add the following code to the `<nav>` tag in **dashboard.js**
```
<a
 href='/dashboard/<name-of-tab>/<name-of-first-subroute>
 id='users'
 className={location.pathname.includes('/dashboard/<name-of-tab>') ? 'active' : null} >
<name-of-tab>
</a>
```
Create a new folder named **<name-of-tab>** for the tab in the DashboardTabs folder with the following content.

  - Create Subfolder `<name-of-tab>` Options
  - Create `<name-of-tab>.js`
  - Create `<name-of-tab>.css`
  - Create `routes.js`

- ### New dashboard tab sub-route component :

**Follow this basic syntax for each component which has its own route.**
```
class <Component> extends Component {   
    render() {
       return (
           <Layout>
               <Content className='content'>
                   //Body
               </Content>
           </Layout>
        )
   }
}
export default <Component>
```
        
    
     



