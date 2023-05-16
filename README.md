# Docker Compose Templates

This repository contains a collection of Docker Compose templates that I use to set up various services on my server. I created this repository to make it easier to set up these services on new servers, and to share my configurations with others. 

## Structure

Each subdirectory in this repository represents a different service or stack. 

```bash
.
├── postgres
│   ├── docker-compose.yml
│   └── README.md
├── redis
│   ├── docker-compose.yml
│   └── README.md
└── ...
README.md
```

Inside each subdirectory, you will find a `docker-compose.yml` file, which contains the Docker Compose configuration for that service, and a `README.md` file, which provides instructions and information specific to that service.

## How to Use

1. Clone this repository: `git clone https://github.com/yourusername/docker-compose-templates.git`
2. Navigate into the directory of the service you want to set up: `cd docker-compose-templates/postgres`
3. Run Docker Compose: `docker-compose up -d`

## Services

Here are the services currently available in this repository:

- [x] [Postgres](postgres/)
- [ ] [Redis](redis/)

...and more!

## Contributions

Contributions are welcome! Please feel free to submit a pull request.

## License

This repository is licensed under the MIT License.