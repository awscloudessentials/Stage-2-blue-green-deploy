# Stage-2-blue-green-deploy
This project demonstrates a Blue/Green deployment pattern using Docker Compose and Nginx as a reverse proxy and failover controller.

It runs two identical Node.js services (Blue & Green) as pre-built Docker images.
Nginx routes traffic between them, serving all requests from Blue by default and automatically failing over to Green if Blue becomes unavailable.

The goal is zero downtime deployments with automated health-based failover and header-preserving traffic routing.
