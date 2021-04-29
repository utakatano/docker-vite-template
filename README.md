# Vite Template with Docker/Docker Compose

This is Vite template without installing node.js in local.

## Environment

- Node.js ... 16.0.0
- [Vite](https://vitejs.dev/) ... 2.2.3

## How to run local development

You can only run the following commands and see `http://localhost:8080` in your browser after build is done.

```sh
% docker-compose up -d --build

% docker-compose exec develop bash

# in the container
/app＃ cd my-vue-app
/app/my-vue-app＃ npm install # if node_modules does not exist
/app/my-vue-app＃ npm run dev
```

## How to create your new project

Please follow the step [the link in official Vite site](https://vitejs.dev/guide/#scaffolding-your-first-vite-project).

```sh
% docker-compose up -d --build

% docker-compose exec develop bash

# in the container
# https://vitejs.dev/guide/#scaffolding-your-first-vite-projects
/app＃ npm init @vitejs/app {project_name} -- --template {template_name}
```