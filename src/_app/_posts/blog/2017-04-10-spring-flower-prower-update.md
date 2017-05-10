---
layout: post
title: Spring Flower Power Updates
category: blog
---

It's flower power time ! And the good time for a global package update on all our docker images.
Re-pull images to get the updated version !

# New docker images

[Mailtrain](https://github.com/osixia/docker-mailtrain)

[www-redirect](https://github.com/osixia/docker-www-redirect)

[Ssl-helper](https://github.com/osixia/docker-ssl-helper)

[postfix-gateway](https://github.com/osixia/docker-postfix-gateway)

# Deleted docker images

postfix-gateway-confd: is now [postfix-gateway](https://github.com/osixia/docker-postfix-gateway) confd is not used anymore.

Gitlab: we now use the awesome [sameersbn/gitlab](https://hub.docker.com/r/sameersbn/gitlab/) image without extending it to add light-baseimage's tools.
The tools we need are now run by [init containers](https://kubernetes.io/docs/concepts/workloads/pods/init-containers/) on our kubernetes cluster.
