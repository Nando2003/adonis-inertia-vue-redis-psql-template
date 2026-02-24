## How to run it in development mode

1. Copy the `.env.example` file to `.env` and set your environment variables:

   ```bash
   $ cp .env.example .env
   ```

2. Install the dependencies:

   ```bash
   $ npm install
   ```

3. Add your `APP_KEY` by running:

   ```bash
   $ node ace generate:key
   ```

4. Start the development environment using Docker Compose:

   ```bash
   $ docker compose up --build
   ```

## How to run it in production mode

1. Make sure to set the `NODE_ENV` variable to `production` in your `.env` file:

   ```env
   NODE_ENV=production
   ```

2. Build and start the production environment using Docker Compose:

   ```bash
   $ docker compose -f docker-compose.prod.yml up --build
   ```
