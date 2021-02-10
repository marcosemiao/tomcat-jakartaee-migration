# Tomcat Migration Tool for Jakarta EE - Changelog

## 0.2.0 (in progress)

- Add this changelog (markt)
- Update dependencies (Apache Commons IO 2.8.0, Apache Ant 1.10.9) (markt)
- Fix [#9](https://github.com/apache/tomcat-jakartaee-migration/issues/9). Exclude the `javax.xml.namespace` package in the EE profile (ebourg)
- Include the `javax.management.j2ee` package in the EE profile (ebourg)
- Add a test to confirm `javax.xml.xpath.XPathConstants` is not converted (ebourg)
- Update README to mention the tool is now available on Debian/Ubuntu (ebourg)
- Include the `javax.security.enterprise` package in the EE profile (ebourg)
- Include the `javax.xml.registry` package in the EE profile (ebourg)
- Include the `javax.security.jacc` package in the EE profile (ebourg)
- Include the `javax.faces` package in the EE profile (ebourg)
- Include the `javax.batch` package in the EE profile (ebourg)
- Include the `javax.jws` package in the EE profile (ebourg)
- Include the `javax.resource` package in the EE profile (ebourg)
- Fix [#7](https://github.com/apache/tomcat-jakartaee-migration/issues/7). Include the `javax.jms` package in the EE profile (alitokmen/mgirgorov)
- Make `migrate.sh` work from any path (mgrigorov)
- Add a new option `-zipInMemory` that processes archives (ZIP, JAR, WAR, etc.) in memory rather via a streaming approach. While less efficient, it allows archives to be processed when their structure means that a streaming approach will fail. (markt)
- Include the Maven Wrapper source files in the source distribution. (markt)
- Ensure that all the Manifest attributes are processed during the migration process. (markt)
- Include `.properties` and `.json` files in the conversion process. (markt)
- Replace `-verbose` with `-logLevel=` to provide more control over logging level. (markt)
- Fix [#13](https://github.com/apache/tomcat-jakartaee-migration/issues/13). Refactor mapping of log messages to log levels. (markt)
- Fix [#3](https://github.com/apache/tomcat-jakartaee-migration/issues/3). Add support for excluding files from conversion. (markt)
- Fix handling of classes with more than 32768 entries in the constant pool. (markt)

## 0.1.0

- Initial release (markt)