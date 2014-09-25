Changelog stomp-php
-------------------

2.1.0
-----

2.1.0 based fork
----------------

- fixed travis ci setup
- added more unit tests (removed ssl unti tests, they don't depend on stomp client)
- refactoring extracted Connection, Parser, Protocol, ActiveMq, RabbitMq, ConnectionException, ErrorFrameException, UnexpectedResponseException
- fixed dead loops caused by connection exceptions
- removed the posibillity to auto-reconnect outside the connect process (it's quite intransparent and can lead to much more problems than expected)
- added a read buffer seen at https://github.com/camronlevanger/stomp-php/commit/8bca4a55b5db8493f543c7f2d1db13d42455e19d

