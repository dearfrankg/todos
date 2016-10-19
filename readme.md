
# Meteor Todos App

#### Creating the app

| Task with diff link | Description     |
| :------------- | :------------- |
| [create app][create]                      | - create app: `meteor create simple-todos`<br>- install packages: `meteor npm install`       |
| [configure for components][components]    | - add packages: `meteor npm install --save react react-dom`<br>- replace the starter code (html, js, css)<br>- add `App` and `Task` components       |
| [configure for collections][collections]  | - create tasks collection `imports/api/tasks.js`<br>- load tasks collection on the server `server/main.js`<br>- use data from a collection inside components<br>- insert task from the console: `meteor mongo`        |
| [forms and events][forms]                 | - add task form<br>- add submit handler<br>- sort tasks by time      |
| [update and remove][update]               | - update task with checkbox and delete button<br>- add handlers: toggleChecked and deleteTask       |
| [hide completed with temp UI state][hide] | - set initial UI state for `hideCompleted`<br>- add hide completed checkbox<br>- add toggleHideCompleted handler<br>- filter tasks in renderTasks<br>- update data container to return incompleteCount<br>- display incompleteCount in the header      |
| [user accounts]                           | - add packages: `meteor add accounts-ui accounts-password`<br>- create Accounts UI wrapper component<br>- include sign in form<br>- configure accounts-ui in `imports/startup/accounts-config`<br>- import accounts configuration in `client/main.js`<br>- add user-related functionality       |
| [security with model methods][security]   | - remove package: `meteor remove insecure`<br>- add methods for `add`, `remove`, `update` task `imports/api/tasks`<br>- update components to use new methods<br>- `Optimistic UI` will update the UI immediately and roll-back on error        |
| [filter data with pub/sub][filter]        | - remove package: `meteor remove autopublish`<br>- add publication for tasks `imports/api/tasks`<br>- subscribe to tasks in App container `imports/ui/App`<br>- add a button to make tasks private<br>- add package: `meteor npm install --save classnames`<br>- selectively publishing tasks based on privacy status<br>- add extra method security in `imports/api/tasks`       |
| [testing]                                 | - add package: `meteor add practicalmeteor:mocha`<br>- test app: `meteor test --driver-package practicalmeteor:mocha`<br>- add a scaffold for a method test<br>- prepare the database for each test<br>- add test to check delete method       |
| [performance]                             | - add package: `meteor npm install --save bcrypt`        |




[create]: https://github.com/dearfrankg/todos/commit/da2fbf2f863cf81fbcbc3009c97784ee265baa01
[components]: https://github.com/dearfrankg/todos/commit/ada0f954ab8b960e8983936e7f25de1a9ac0252f
[collections]: https://github.com/dearfrankg/todos/commit/743614db922a05ccbd9715661219fb00bbe0c750
[forms]: https://github.com/dearfrankg/todos/commit/89dff50a4ba5197e1ae476b3eff30b3c46bee103
[update]: https://github.com/dearfrankg/todos/commit/b225080e2f566d75f2ee60d3f44f0e94b45b7fb3
[hide]: https://github.com/dearfrankg/todos/commit/e4e0b905eda7c0afd68dcfa76efbfa3fad38bde7
[user accounts]: https://github.com/dearfrankg/todos/commit/7a0e2c920fa06e0083148fa7b23ab6bd7111dbde
[security]: https://github.com/dearfrankg/todos/commit/f261a2cbf557dc31b0029c69160fa66db9bcf0b9
[filter]: https://github.com/dearfrankg/todos/commit/adaafed9945f744d5d71d5e2a4ec9c785b346641
[testing]: https://github.com/dearfrankg/todos/commit/b14ba383cc1e0df078524cc4053ff2705e5aa63d
[performance]: https://github.com/dearfrankg/todos/commit/f65a8b62e7e1bd59d1f7f6b7b6d93dd4921fcbfd
