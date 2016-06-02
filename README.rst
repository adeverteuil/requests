Requests: HTTP for Humans
=========================

This fork has a quickfix for upstream issue
`#3222 Session.request() overrides socket.setdefaulttimeout()
<https://github.com/kennethreitz/requests/issues/3222>`_.

The upstream project's devs are already aware of the problem. They have
design compromises to discuss which explains why a permanent fix is not
released yet. However I need this fix now because an in-house system I
maintain uses a library which in turn uses requests so I can't set the
timeout in my own code.
