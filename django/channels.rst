Django and WebSockets with channels
- WebSockets  -> Protocol 
- Channels -> pip install channels and add it to your INSTALLED_APPS += "channels"
- Apply migrate command
- Define ASGI_APPLICATION in settings and change asgi file with channels ProtocolTypeRouter to router different Protocols Http and Websocket 

- Consumer just like Django Application for just specific client connected peer to peer
- Channel layer broadcast to a group
- worked only with 3.0.4 and 3.0.5 


For Streaming review this:
- review this https://github.com/NeuralNine/vidstream/blob/main/vidstream/streaming.py
