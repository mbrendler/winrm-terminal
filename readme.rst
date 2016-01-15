winrm_cmd
=========

Install dependencies::

  $ pip install pywinrm


Run command::

  $ ./winrm_cmd my-user:my-password@my-host[:my-port] COMMAND [ARGS..]

You can add a ``~/.winrm.json`` with credentials::

  {
    "my-label": {
      "host": "my-host:my-port",
      "user": "my-user",
      "password": "my-password"
    }
  }

Now you can run a command the following way::

  $ ./winrm_cmd my-label COMMAND [ARGS..]
