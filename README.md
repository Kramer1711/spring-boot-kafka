# spring-boot-kafka

# kafka配置

config/server.properties

 ############################# Socket Server Settings #############################
 # The address the socket server listens on. It will get the value returned from 
 # java.net.InetAddress.getCanonicalHostName() if not configured.
 #   FORMAT:
 #     listeners = listener_name://host_name:port
 #   EXAMPLE:
 #     listeners = PLAINTEXT://your.host.name:9092
 #listeners=PLAINTEXT://:9092
 listeners=PLAINTEXT://{内网ip}:9092

 # Hostname and port the broker will advertise to producers and consumers. If not set, 
 # it uses the value for "listeners" if configured.  Otherwise, it will use the value
 # returned from java.net.InetAddress.getCanonicalHostName().
 #advertised.listeners=PLAINTEXT://your.host.name:9092
 advertised.listeners=PLAINTEXT://{外网ip}:9092`
