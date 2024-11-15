### Running the Project

To get started, I recommend [installing pnpm](https://pnpm.io/installation) since it's the package manager used in this repository.

Begin by forking the repository and then cloning it to your local machine:

```
git clone <your-fork>
```

Navigate to the project's root directory:

```
cd ./andri.dev
```

Next, copy the development version of the `env` file:

```
cp ./apps/andri.dev/env.example ./apps/andri.dev/env.local
```

Now, you have the `env.local` file ready for configuration:

```
DATABASE_URL = your-database-connection-string
SALT_IP_ADDRESS = super-secret
```

For the `DATABASE_URL` use your database connection string. I personally use the free version of [MongoDB](https://www.mongodb.com/), and you can do the same by creating a database there and [adding the connection string](https://www.mongodb.com/basics/mongodb-connection-string) to the `env.local`.

As for `SALT_IP_ADDRESS`, feel free to fill it with some of your secret words. It acts as a salt for hashing users' IP addresses.

Once configuration is complete, still at the root of the project directory, install the required dependencies:

```
pnpm install
```

Finally, run the project:

```
pnpm dev
```

Now, your project should be up and running smoothly!
