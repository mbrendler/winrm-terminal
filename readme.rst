winrm
=====

Install dependencies::

  $ pip install pywinrm

Run command::

  $ ./winrm my-user:my-password@my-host[:my-port] COMMAND [ARGS..]

Add credentials to ``~/.winrm.json``::

  {
    "my-label": {
      "host": "my-host:my-port",
      "user": "my-user",
      "password": "my-password"
    }
  }

Now run a command the following way::

  $ ./winrm my-label COMMAND [ARGS..]

See ``./winrm --help`` for more information.

ZSH-completion
--------------

* ZSH completion handles 'destination-lables' from ``~/.winrm.json`` and
  completes commands and arguments from ``~/.winrm.commands``.

* You can add your own commands to ``~/.winrm.commands``.  Every line must be a
  command with its arguments.

* Copy ``zsh_completion/_winrm`` into any ``$fpath`` directory.
