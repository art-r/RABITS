# RABITS
Really Advanced Better InformaTion Sharing


A Project to run the following services:
- Nextcloud (fpm image) (with:)
	- Redis
	- MariaDB
	- Nginx proxy
	- letsencrypt (for ssl certificates)
	- crowdsec (parsing nginx log files)
- tbd 

***
## How to run this
1. Configure the secrets in the `db_secret.conf` file
2. Configure settings in the `nx_compose.yml` file (Look for the `# SET THIS` comment)
3. Run the following command:
```bash
docker-compose up
```
4. If everything works shut it down and now run it in the background:
```bash
docker-compose up -d
```