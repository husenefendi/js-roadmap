# Contribution Guidelines
Please note that this project is released with a [Contributor Code of Conduct](code-of-conduct.md). By participating in this project you agree to abide by its terms.

## Folder Structur
if you want to add new module, you can put in **modules/[category]/** folder
and use [snake case](https://betterprogramming.pub/string-case-styles-camel-pascal-snake-and-kebab-case-981407998841) or [Camel Case](https://betterprogramming.pub/string-case-styles-camel-pascal-snake-and-kebab-case-981407998841#:~:text=Camel%20Case%20(camelCase)) for naming file and folder .
<br/>
<br/>
```js
├── code-of-conduct.md
├── contributing.md
├── LICENSE
├── modules // modules location
│   ├── 01.Basic //category
│   │   ├── 01.git.md  //modulte detail
│   │   ├── 02.Variable_data_types.md
│   │   └── readme.md
│   ├── 02.ApiConcept
│   │   └── readme.md
│   ├── 03.ReactJS
│   │   └── readme.md
│   ├── 04.ReactNative
│   │   └── readme.md
│   └── 05.AdvanceReact
│       └── readme.md
├── readme_backup.md
└── readme.md
```
<br/>
<br/>

## Adding something to this Road Map

If you have something module to contribute to an roadmap, this is how you do it.

You'll need a [GitHub account](https://github.com/join)!.
and craate yout [**Pull Request**](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) or follow this step

### Code Contributions 

1. fork the repository on GitHub
2. Clone your repository have been forked
3. update some content/codes
4. push to your repository have been forked
5. create `pull request` and the target will assign to main repo.


### Update your repo
before we update your repo have been forked, you need to update first, follow this step to update/rebase your local repo
```clis
$ git remote add upstream git@github.com:husenEF/js-roadmap.git
$ git fetch upstream
$ git rebase upstream/main
$ git push origin main --force
```

<br/>

### Add new
i like git workflow from [nvie](https://nvie.com/posts/a-successful-git-branching-model/), they have status like `feature`, `hotfix` and `release`.
you can put `hotfix`, `feature` on your branch name

```cli
// create new branch
$ git checkout -b feature/[category][module_name] 

```
**branch name**: 
 - category : Basic, Api Concept, React JS, React Native or Advance React
 - modules name : container **number** & **title**
 - see [folder structur](#folder-structur)

<br/>
<br/>

### Update or Fix

```bash
//update or hotfix
$ git checkout -b hotfix/[category][module_name]
```

<br/>
<br/>

### Push

after finish your modules, you can push to your branch and make **Pull Request**. 
but, make sure your branch updated with main branch. go to Project page, and click **pull request**

![Screenshot from 2022-04-24 12-54-53](https://user-images.githubusercontent.com/91042496/164958722-ca71d69b-a68a-4f82-832c-3e1857b0cee3.png)


**Update with main branch**'
1. Merge (execute from the branch)
    ```
    $ git pull (or git fetch)
    $ git merge origin/develop
    $ git push
    ```
2. Rebase (execute from the branch)
   ```
   $ git pull --rebase (or git fetch)
   $ git rebase origin/develop
   $ git push --force (or git push -f)
   ```

**Create Pull Request**

![image](https://user-images.githubusercontent.com/546566/164817281-91a1497e-f824-473a-9018-3de8700e5b1a.png)

if you have some branch, yout branch will appear like this:
![image](https://user-images.githubusercontent.com/546566/164817451-5077e34a-38ca-4315-b2d6-3a68655e469b.png)

then, you can clik **Compare & pull request** and you will page for create new pull request. You can chosse **Reviewers** and also the someone to merge your Pull request in **Assignees Section**.
update your Detail. what do you update ,for example:
```
New Modules:
- int.md
- var.md

or

update/fix module:
- int.md
- var.md
```
![image](https://user-images.githubusercontent.com/546566/164817559-dae1466e-d415-45da-a77f-856d5ea92f95.png)

and click button `Create pull Request` and waiting your pull request is accepted