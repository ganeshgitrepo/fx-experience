Maven
===
Add to your maven settings.xml the system dependent property jfx-runtime, something like this:
```xml
<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0
                      http://maven.apache.org/xsd/settings-1.0.0.xsd">

  ...
  <profiles>
    ...
    <profile>
      <id>default</id>
	<properties>
          <fx.home>C:/Program Files/Java/jre7/lib</fx.home>
	</properties>
    </profile>
  </profiles>

  <activeProfiles>
    <activeProfile>default</activeProfile>
  </activeProfiles>
</settings>
```

Demo
===
build jar and start demo main class:

Swing Demo App:
`org.comtel.javafx.SwingMainDemo`

JavaFX Demo App:
`org.comtel.javafx.MainDemo`

License
===
new BSD License
