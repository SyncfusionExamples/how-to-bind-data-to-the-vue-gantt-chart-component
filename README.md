# Vue Gantt Chart Data Binding Example

This repository contains a Vue 3 app that binds a Syncfusion Gantt chart to remote task data using `DataManager` and `WebApiAdaptor`.

## Project overview

The app renders a Syncfusion `<ejs-gantt>` chart in `src/App.vue` with columns for Task ID, Task Name, and Start Date. It loads hierarchical task data from a remote endpoint.

## Key files

- `src/App.vue`
  - Renders the Gantt chart and maps fields such as `TaskId`, `TaskName`, `StartDate`, `EndDate`, `Duration`, `Progress`, `Predecessor`, and `SubTasks`.
- `src/main.js`
  - Creates the Vue app and registers a Syncfusion license.
- `src/data.js`
  - Includes local sample data (`projectNewData`, `selfData`) not currently used.
- `src/components/HelloWorld.vue`: default Vue CLI starter.

## Dependencies

- `vue` `^3.2.13`
- `@syncfusion/ej2-vue-gantt` `^21.1.38`
- `core-js`

## Setup

1. Install dependencies:

```bash
npm install
```

2. Run the app:

```bash
npm run serve
```

3. Open the local site in your browser:

```text
http://localhost:8080/
```

## Notes

- The current code uses remote data via `DataManager` and `WebApiAdaptor`.
- `src/data.js` contains local sample data not imported into `App.vue`.

## Links

- Syncfusion Gantt docs: https://ej2.syncfusion.com/vue/documentation/gantt/data-binding
- Remote data demo: https://ej2.syncfusion.com/vue/demos/#/material/gantt/remote-data.html
