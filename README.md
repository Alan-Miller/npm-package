# npm package

## Symlink
A symlink to the package folder allows the module to be loaded from anywhere on the computer. The linked module can then be required in a project from anywhere on the computer. Any change made in the module will then be automatically reflected in the project.

#### **Create symlink**
- In folder where package is:
  ```sh
  npm link 
  ```

#### **Remove symlink**
- In folder where package is:
  ```sh
  npm unlink 
  ```

- If a previous link was made and you want to remove it but not remove a new link that was made, and if the original link continues to work after running `npm unlink` and then `npm link` again, you can just remove the old link manually.
  
  In `~/node/bin`:
  ```sh
  ls -al # see all links
  rm link_name # remove link
  ```

#### **Show path to global node_modules folder**
```sh
npm root -g
```

#### **Install command globally** 
Link the script to a location on the path so it can be used like any other shell command.
```sh
npm i -g
```