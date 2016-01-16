winrm
=====

Install dependencies::

  $ pip install pywinrm


Run command::

  $ ./winrm my-user:my-password@my-host[:my-port] COMMAND [ARGS..]

You can add a ``~/.winrm.json`` with credentials::

  {
    "my-label": {
      "host": "my-host:my-port",
      "user": "my-user",
      "password": "my-password"
    }
  }

Now you can run a command the following way::

  $ ./winrm my-label COMMAND [ARGS..]
