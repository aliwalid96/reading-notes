# Configuring Django Settings: Best Practices

### Managing Django Settings: Issues

Usually, you have several environments: local, dev, ci, qa, staging, production. Each environment can have its own specific settings . You need an approach that allows you to keep all these Django setting configurations.

Sensitive data. You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.


Sharing settings between team members. You need a general approach to eliminate human error when working with the settings. For example, a developer may add a third-party app or some API integration and fail to add specific settings. On large (or even mid-size) projects, this can cause real issues.


Django settings are a Python code. This is a curse and a blessing at the same time. It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.



12 Factors
12 Factors is a collection of recommendations on how to build distributed web-apps that will be easy to deploy and scale in the Cloud. It was created by Heroku, a well-known Cloud hosting provider.

As the name suggests, the collection consists of twelve parts:

Codebase
Dependencies
Config
Backing services
Build, release, run
Processes
Port binding
Concurrency
Disposability
Dev/prod parity
Logs
Admin processes

Each point describes a recommended way to implement a specific aspect of the project.

### django-environ

Based on the above, we see that environment variables are the perfect place to store settings.

riting code using os.environ could be tricky sometimes and require additional effort to handle errors. It’s better to use django-environ instead.

Technically it’s a merge of:

envparse
honcho
dj-database-url
dj-search-url
dj-config-url
django-cache-url


## Django Settings: Best practices
Keep settings in environment variables.
Write default values for production configuration (excluding secret keys and tokens).
Don’t hardcode sensitive settings, and don’t put them in VCS.
Split settings into groups: Django, third-party, project.
Follow naming conventions for custom (project) settings.

# What Is SSH?

SSH, or Secure Shell Protocol, is a remote administration protocol that allows users to access, control, and modify their remote servers over the internet.


SSH service was created as a secure replacement for the unencrypted Telnet and uses cryptographic techniques to ensure that all communication to and from the remote server happens in an encrypted manner. It provides a mechanism for authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client.



The SSH key command instructs your system that you want to open an encrypted Secure Shell Connection. {user} represents the account you want to access. For example, you may want to access the root user, which is basically synonymous with the system administrator with complete rights to modify anything on the system. {host} refers to the computer you want to access.

## Understanding Different Encryption Techniques

The significant advantage offered by SSH over its predecessors is the use of encryption to ensure a secure transfer of information between the host and the client

1. Symmetrical encryption
2. Asymmetrical encryption
3. Hashing

## Symmetric Encryption
Symmetric encryption is a form of encryption where a secret key is used for both encryption and decryption of a message by both the client and the host

## Asymmetric Encryption
Unlike symmetrical encryption, asymmetrical encryption uses two separate keys for encryption and decryption


## Hashing
One-way hashing is another form of cryptography used in Secure Shell Connections. One-way-hash functions differ from the above two forms of encryption in the sense that they are never meant to be decrypted.


### How Does SSH Work With These Encryption Techniques
The way SSH works is by making use of a client-server model to allow for authentication of two remote systems and encryption of the data that passes between them.
