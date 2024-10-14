# Caching Proxy Server

A  caching proxy server built with Node.js, Express, Axios, and NodeCache. The server forwards requests to an origin server and caches the responses to improve performance and reduce the load on the origin server.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- **Node.js**: Make sure you have Node.js installed. You can download it from the [Node.js official website](https://nodejs.org/).
- **npm**: npm is typically installed with Node.js. You can verify the installation by running the following commands:

  ```bash
  node -v
  npm -v
  ```

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Redgerd/caching-server.git
   cd caching-proxy
   ```

2. Install the dependencies:

   ```bash
   npm install
   ```

## Usage

### Starting the Caching Proxy Server

To start the caching proxy server, run the following command:

```bash
node ./index.js start --port <number> --origin <url>
```

- `--port`: The port on which the caching proxy server will run.
- `--origin`: The URL of the origin server to which the requests will be forwarded.

#### Example:

```bash
node ./index.js start --port 3000 --origin http://dummyjson.com
```

In this example, the server will start on port 3000 and forward requests to `http://dummyjson.com`.

### Clearing the Cache

You can clear the cache by running the following command:

```bash
node ./index.js clear-cache
```

## Additional Resources

For more information on caching servers and implementation tips, check out:

- [Roadmap to Caching Servers](https://roadmap.sh/projects/caching-server)
