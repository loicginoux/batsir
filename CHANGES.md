0.3.4
-----------
- Fixed issue when using bunny 0.9.0.pre9. Bunny::Session#start now returns ifself instead of its channel.


0.3.3
-----------
- Bunny :heartbeat option is now explicitly set. It defaults to 0; the original AMQP 0.8 setting.


0.3.2
-----------
- Filters can now be passed initialisation options


0.3.1
-----------
- Renamed config variable 'connection_pool_size' to a more apt 'amqp_pool_size'


0.3.0
-----------
- AMQPAcceptor and AMQPNotifier classes now only support Bunny 0.9 and up.
  This fixes a bug that occurred when talking to an AMQP 0.9 server with a Bunny 0.8 client.
  High message rates would, at some point, cause the server to reject all messages.


0.2.1
-----------
- Notifiers will not modify the message
- FieldTransformers now always return message hashes with strings for keys


0.2.0
-----------
- first production-ready code
