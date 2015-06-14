
Does Read the Docs have pandoc installed?

.. runblock:: pycon

    >>> import os
    ... from subprocess import check_output, CalledProcessError
    ... try:
    ...     print(check_output(['pandoc', '--version']))
    ... except CalledProcessError:
    ...   print("No pandoc on %s" % os.environ['PATH'])

