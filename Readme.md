# 🚀 HTML Page Deployed with Docker

This is a simple static HTML page deployed using a Docker container with the official Nginx image.

## 📂 Project Structure

- index.html: The static HTML file.
- No custom Dockerfile was needed – we used volume mounting with the official nginx image.

## 🐳 Docker Command Used

```bash
docker run -it -d --name html -p 8080:80 -v /home/ubuntu/website:/usr/share/nginx/html nginx
