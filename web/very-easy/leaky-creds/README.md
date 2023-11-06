# Leaky-Creds

This challenge simulates a developer leaving sensitive information within the comments of an HTML page.

## Challenge Information

- **Category:** Web
- **Points:** 10
- **Difficulty:** Very Easy
- **Author:** [Ryan McMillan](https://github.com/rmcmillan34/)

## Description

You are to analyse this website to find sensitive information that the lazy developers have left out in the open.

## Setup

- **Requirements:** The only required software to solve this challenge is a web browser.
- **Docker:** 
1. Clone the repository
```bash
git clone https://github.com/rmcmillan34/ctf-challenges
```

2. Build the Docker image
Navigate to the leaky-creds directory containing the Dockerfile and the `index.html` file for the challenge.

```bash
docker build -t leaky-creds .
```

3. Run the Docker Container
start the container and expose it on a specific port (e.g., port 8080)

```bash
docker run -d -p 8080:80 leaky-creds
```

4. Access the challenge
The challenge is now running and can be accessed by opening a web browser and accessing `http://localhost:8080`. Participants will see the web page that is leaking sensitive information.

## Flag

- `RS{SPRUNG_4_L34K}`

## Solution

**Hint 1**: I heard someone comment how lazy @rmcmillan34 is of a developer

**Hint 2**: Use the tools of a developer to help solve this challenge

Utilise your browser's developer tools to view the source code of this website. Read the comments on the source code to find the flag.

## License

This repository is licensed under the [MIT License](/LICENSE).

## Contributing

See the [ctf-challenges/README.md](/README.md) for guidelines on how to contribute to this project


