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
