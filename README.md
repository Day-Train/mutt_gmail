# mutt_gmail
Ansible role that installs mutt on Ubuntu Linux or FreeBSD and configures mutt email client to work with a user's Gmail account.

## Requirements
This role requires root access so your playbook should be invoked with appropriate privilege escalation such as `become`. The user must also have a valid Gmail account. Be aware that Gmail may require you to create/sign-in with a special app password for your host.

## Role Variables
Variables you will have to configre are listed below. See `defaults/main.yml`:

	mg_user: john
	mg_email: john_smith@gmail.com
	mg_name: "John Smith"
	mg_google_app_pass: password
	mg_smtp_url: smtp://john_smith@smtp.gmail.com:587/

> Note: This role expects the mg_user to match the username to appropriately install the configuration file in the user's home directory.

## Dependencies
None

## License
BSD

## Author Information
This role was created in 2017 by Alex Day.
