

# Push an image to GitHub Packages (GHCR)

1. Create image
2. Create PAT (Personal Access Token) on GitHub
3. Authenticate GHCR (GitHub Container Registry)
4. Tag and push our image to GHCR

```sh
export CR_PAT=<TOKEN>
echo $CR_PAT | docker login ghcr.io -u USERNAME --password-stdin
```

# Use GitHub Actions to Publish a Docker image to GitHub Packages (GHCR)

1. Create repo - and Checkin our Dockerfile
2. Build your GitHub action workflow
3. Trigger our workflow
