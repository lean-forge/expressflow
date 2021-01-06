<br/>
<br/>
<p align="center">
  <img src="./media/ef-banner.jpg" />
</p>
<br />
<br />
<h2 align="center" >
    expressFlow
</h2>
<h3 align="center" >Destitutus ventis, remos adhibe</h3>
<br />
<br />
<br/>
<br/>
<br />

## Admins

| Name          | Mail                |
| ------------- | ------------------- |
| Tom Schönmann | tom@expressflow.com |

## Developing

### Branches

- `main` is the current working branch, containing all latest changes
- `dev/production` contain the latest changess for internal review/all users

---

### Working on issues

1. create new branch from `main`
2. naming for branch according to issue type:
```
- bugfix/[issue-nr]-title-of-branch
- feature/[issue-nr]-title-of-branch
- enhancement/[issue-nr]-title-of-branch
 ```
3. Commit changes to your branch
4. Draft a new pull request (`PR`) when you're ready to review your changes:
```
- select members for review, at least one
- select related issue
```
5. Enter text into input field of PR according to this schema:
```
### Goals

- required, short description of what this PR changes

### Notes

- optional, adding more context that might be relevant
```
6. Open PR
7. Commit changes after feedback & merge PR into master

---

### Styling

- we're using `prettier` for all styling
- prettier is installed as a dev dependency in all our repos, so no global install required
- good use: activate "format on save" in your IDE

---

### Linting

- we're using pre-configured linting sets by CRA, Firebase, etc

---

### Documentation & code comments

- comment your code according to JSDoc-schema:
```
/**
 * I'm a multine comment, default for function documentation.
 */
function fn(){
  // I'm an inline comment, default for comments inside functions,
  // classes, etc. Not used for documentation
}

export interface Interface {
  /** I'm a short single line comment for documentation */
  a: string;
  
  /**
   * I'm a multiline comment for documentation,
   * b/c my text is longer than one line can hold.
   */
  b: string;
}
```
