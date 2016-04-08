# Installation

- [Installation](#installation)
    - [Server Requirements](#server-requirements)
    - [Installing SocietyCMS](#installing-societycms)

<a name="installation"></a>
## Installation

<a name="server-requirements"></a>
### Server Requirements

SocietyCMS has a few system requirements. They are mostly the same as those from the underlying Laravel Framework with a few exceptions.
If you are setting up a Server, make sure that it meets these requirements:

<div class="content-list" markdown="1">
- PHP 5.5.9 or higher
- OpenSSL PHP Extension
- PDO PHP Extension
- Mbstring PHP Extension
- Tokenizer PHP Extension
- Mcrypt PHP Extension
- GD PHP Library
- MySql 5.5
</div>

In addition, it is highly recommended that you have ond of the following cache driver installed. By default, SocietyCMS will not use any caching.
<div class="content-list" markdown="1">
- memcached
- redis
</div>

<a name="installing-societycms"></a>
### Installing SocietyCMS

SocietyCMS utilizes [Composer](http://getcomposer.org) to manage its modules and all the dependencies. So, before using SocietyCMS, make sure you have Composer installed on your machine.

    composer create-project societycms/societycms your-project-name

Composer will now download all the required dependencies. After the installation has finished, change into your project directory and run the install command:

    php artisan societycms:install

This will perform the following cations:
<div class="content-list" markdown="1">
- Setup database information
- Running migrations
- Running seeds
- Publishing assets
- Create a first admin account
</div>