# Git Hooks for Laravel 9 on nginx

- change folder owner
- change folder permission to 775
- clear all caching [cache, view, route, config, event]
- cache [route, config, view, event]
- restart nginx 

# setup

1. copy post-merge to project root .git/hooks/
2. change port-merge file premission 
    - chmod +x post-merge 
3. open post-merge file and edit OWNER and PROJECT_NAME variable 
4. copy post-merge to post-checkout
    - cp post-merge post-checkout
    - change echo parameter post-merge

## **required sudo user**
>after pull or checkout if your user in not root terminal will prompt you for entering a password.