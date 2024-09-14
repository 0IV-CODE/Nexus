# 🎮 NEXUS: 🎮

# 🚀 Project Overview

Every gamer knows the importance of a well-organized inventory. From managing equipment and resources to setting goals and tracking progress, NEXUS is designed to help you stay on top of your game, out of the digital realm where this is very much needed.

# 🛠 Features

👤 **User Management**

- Create and manage your profile.
- Complete with avatars and bios for personalized interaction.

📝 **Activity Logging**

- Track your activities and missions.
- Maintain detailed logs to monitor progress over time.

🎯 **Goal Setting**

- Define your goals and objectives.
- Monitor your progress and achievements with our goal-setting feature.

💵 **Budget Tracking**

- Keep a close watch on your finances.
- Manage necessities, savings, and expenditures with ease.

📊 **Stats Tracking**

- Record and analyze your personal statistics.
- Track health metrics, educational progress, and physical activity levels.

📅 **Government Reminders**

- Stay informed about critical dates.
- Receive reminders for insurance renewals, tax deadlines, and other government-related obligations.

### Stores

- Pinia store modules (`activities.ts`, `auth.ts`, `budget.ts`, etc.) manage state for corresponding features. Each module encapsulates its state management logic, ensuring modularity and separation of concerns.

### Views

- **auth**: Contains components related to authentication (`LoginPage.js`).
- **misc**: Holds miscellaneous components like error pages (`ErrorPg.vue`).
- **pages**: Houses full-page components (`GovernmentPage.vue`, `GoalsPage.vue`, etc.) that serve as routes in the application.
- **homePage.vue**: The main entry point (`App.vue`) serves as the root template and configures global styles and scripts.

### Benefits

- **Logical Grouping**: Organizing components, stores, and views by functionality improves code readability and facilitates collaboration among developers.
- **Scalability**: The hierarchical structure accommodates the addition of new features (`storage`, `budget`, `stats`, `logs`) without cluttering the codebase.
- **Maintainability**: Separation of concerns and adherence to naming conventions (`*.vue` for components, `.ts` for TypeScript files) simplify debugging and updates.
- **Convention Over Configuration**: Following Vue.js best practices ensures consistency and makes it easier for new team members to understand and contribute to the project.

This structure promotes efficient development practices and enhances the overall robustness of the Vue.js application, aligning with industry standards and fostering a clear, organized codebase.

## Technology Stack

### Frontend Framework

🖥️ **Vue.js**

- Foundation of the project.
- Provides reactive data binding and efficient rendering for building robust and responsive user interfaces.

### Backend

🌐 **PocketBase**

- Lightweight backend solution.
- Features SQLite database, realtime subscriptions, integrated authentication, and a REST-ish API for efficient data management.

### Version Control

🔄 **GitHub Desktop**

- Facilitates version control and collaboration with Git, ensuring codebase integrity and team coordination.

## Dependencies:

1. "@mdi/js": "^7.4.47",
2. "gsap": "^3.12.5",
3. "pinia": "^2.1.7",
4. "pocketbase": "^0.21.3",
5. "vue": "^3.4.21",
6. "vue-router": "^4.3.0",
7. "vue3-toastify": "^0.2.1",
8. "vuetify": "^3.6.9"

### Dependencies Explanation

1. **"@mdi/js": "^7.4.47"**

   - **Purpose**: Provides Material Design Icons as SVGs or fonts.
   - **Suitability**: Ideal for enhancing the visual appeal and usability of the application with Material Design icons, ensuring consistency and familiarity in UI elements.
   - **Link**: [Material Design Icons](https://materialdesignicons.com/)

2. **"gsap": "^3.12.5"**

   - **Purpose**: GreenSock Animation Platform for high-performance animations.
   - **Suitability**: Essential for creating fluid animations within the application, enhancing user experience and interaction design without compromising performance.
   - **Link**: [GreenSock](https://greensock.com/docs/)

3. **"pinia": "^2.1.7"**

   - **Purpose**: State management library for Vue 3.
   - **Suitability**: Perfect fit for managing application-wide state in a reactive and efficient manner, ensuring scalability and maintainability as the project grows.
   - **Link**: [Pinia](https://pinia.esm.dev/)

4. **"pocketbase": "^0.21.3"**

   - **Purpose**: Backend solution with SQLite database and realtime subscriptions.
   - **Suitability**: Provides a lightweight yet powerful backend for storing application data with realtime capabilities, integrated authentication, and a REST-ish API, suitable for both development and production stages.
   - **Link**: [PocketBase](https://pocketbase.io/)

5. **"vue": "^3.4.21"**

   - **Purpose**: Core Vue.js framework.
   - **Suitability**: Foundation of the project, offering reactive data binding, component-based architecture, and efficient rendering, essential for building robust and responsive user interfaces.
   - **Link**: [Vue.js](https://vuejs.org/)

6. **"vue-router": "^4.3.0"**

   - **Purpose**: Official router for Vue.js applications.
   - **Suitability**: Enables navigation between different views or pages in the single-page application (SPA), ensuring smooth user experience and proper URL handling for different application states.
   - **Link**: [Vue Router](https://router.vuejs.org/)

7. **"vue3-toastify": "^0.2.1"**

   - **Purpose**: Toast notifications for Vue 3 applications.
   - **Suitability**: Provides non-intrusive notifications for various user actions or system events, enhancing user feedback and interaction without disrupting the user experience.
   - **Link**: [Vue3 Toastify](https://github.com/ndelev/vue3-toastify)

8. **"vuetify": "^3.6.9"**
   - **Purpose**: Material Design component framework for Vue.js.
   - **Suitability**: Offers pre-designed components and styles following Material Design guidelines, streamlining UI development and ensuring consistency in appearance and behavior across the application.
   - **Link**: [Vuetify](https://vuetifyjs.com/)

These dependencies are carefully chosen to leverage the strengths of Vue.js ecosystem, enhancing development efficiency, user interface design, state management, animation capabilities, backend integration, and overall user experience in your project.

# 📋 Getting Started

Ready to dive in? Here's how to get started:
This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```

## PocketBase Integration

Please keep in mind that PocketBase is still under active development and full backward compatibility is not guaranteed before reaching v1.0.0. PocketBase is not recommended for production-critical applications yet, unless you are fine with reading the changelog and applying some manual migration steps from time to time.

PocketBase is an open source backend consisting of an embedded database (SQLite) with realtime subscriptions, built-in auth management, convenient dashboard UI, and a simple REST-ish API.

## Getting Started with PocketBase

The easiest way to get started is to download the prebuilt minimal PocketBase app.
please follow the url to the latest PocketBase executable for your OS (operating system):
➼ [PocketBase Docs](https://pocketbase.io/docs/)

Once you've extracted the archive, you can start the application by running:

```sh
./pocketbase serve
```

## PocketBase Routes

- ➼ http://127.0.0.1:8090 - If pb\*public directory exists, serves the static content from it (HTML, CSS, images, etc.)
- ➼ http://127.0.0.1:8090/*/ - Admin dashboard UI
- ➼ http://127.0.0.1:8090/api/ - REST API

When you first access the Admin dashboard UI, you will be prompted to create your first admin account (email and password).

## Data Directories

The prebuilt PocketBase executable will automatically create and manage two new directories alongside the executable:

pb_data - Stores your application data, uploaded files, etc. (usually should be added to .gitignore).
pb_migrations - Contains JS migration files with your collection changes (can be safely committed to your repository).
You can even write custom migration scripts. For more info, check the JS migrations docs.

## Commands

You can find all available commands and their options by running:

```sh
./pocketbase --help
```

or

```sh
./pocketbase [command] --help
```

## Once PocketBase is setup it's as simple as:

```sh
0. Open new terminal in ide
1. cd into "backend"
2. run command "pocketbase serve"
```
