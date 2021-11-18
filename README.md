# How-To-Install-PHP-7.4-on-CentOS-7

## Step 1: Add EPEL and REMI Repository
Run the commands below to add required repositories.

```
sudo yum -y install https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
sudo yum -y install https://rpms.remirepo.net/enterprise/remi-release-7.rpm
```

## Step 2: Install PHP 7.4 on CentOS 7

```
sudo yum -y install yum-utils
sudo yum-config-manager --enable remi-php74
sudo yum update
sudo yum install php php-cli
```

## Use the next command to install additional packages:

```yum install php-xxx```

## Example:

```
sudo yum install php  php-cli php-fpm php-mysqlnd php-zip php-devel php-gd php-mcrypt php-mbstring php-curl php-xml php-pear php-bcmath php-json
```

## The current PHP version should be 7.4.

```
$ php -v
PHP 7.4.0 (cli) (built: Nov 26 2019 20:13:36) ( NTS )
Copyright (c) The PHP Group
Zend Engine v3.4.0, Copyright (c) Zend Technologies
```

To view enabled modules, run:

```php --modules```

You have successfully installed PHP 7.4 on CentOS 7. Enjoy your PHP development/tests with this release and don’t forget to provide feedback to the Development team.
