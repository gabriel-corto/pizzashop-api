Aqui está a versão ajustada do **README** com dicas específicas para usuários de **Windows**:

---

# 🍕 pizza.shop API

Food delivery app (inspired by iFood/Uber Eats) back-end built with TypeScript, Drizzle, and ElysiaJS.

> 🔥 This project aims to be runtime agnostic, meaning it should work on Bun, Node, Cloudflare Workers, or any Web Standard API compatible runtime.

## Running the Project

This project depends on Docker to set up the database. Follow the steps below based on your operating system.

### For Windows Users

If you are using **Windows**, follow these additional steps to set up and run the project smoothly:

#### Step 1: Install Docker Desktop

- Download and install Docker Desktop from [Docker Desktop](https://www.docker.com/products/docker-desktop).
- Make sure **WSL 2** is installed and enabled, as Docker uses it to run on Windows. You can follow the [WSL 2 installation guide](https://docs.microsoft.com/en-us/windows/wsl/install) if needed.
- After installing, **start Docker Desktop** by clicking its icon in the taskbar.

#### Step 2: Clone the Project

Open your terminal and clone the project using Git:

```sh
git clone https://github.com/rocketseat-education/pizzashop-api.git
cd pizzashop-api
```

#### Step 3: Start Docker Containers

Ensure Docker is running. Then, use the following commands to set up the project:

```sh
docker compose up -d
```

This will start the containers required to run the project, including the database (PostgreSQL).

#### Step 4: Install Dependencies

With **Bun** installed, run the following command to install project dependencies:

```sh
bun i
```

#### Step 5: Run Migrations and Seed Data

To create the database tables and populate it with fake data, run:

```sh
bun migrate
bun seed
```

#### Step 6: Run the Application

Finally, start the back-end with:

```sh
bun dev
```

You can now consume the back-end via the front-end or API.

> Note: Every time you want to run the back-end, ensure Docker is running and use `docker compose up -d` to start the required containers.

---

## Features

> The **summary** of the features are listed below. All the features contain E2E tests.

- it should be able to register a new restaurant.
- it should be able to sign in as a restaurant manager.
- it should be able to register as a new customer.
- it should be able to create an order to the restaurant.
- it should be able to manage the restaurant menu.
- it should be able to manage restaurant evaluations.
- it should be able to leave an evaluation.
- it should be able to manage restaurant orders.
- it should be able to update the restaurant public profile.
- it should be able to open/close the restaurant.
- it should be able to list metrics from the restaurant.