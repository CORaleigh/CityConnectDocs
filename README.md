Create and serve up a static html via fuse

In Eclipse:
Create new Dynamic Web Project and check the box to generate web.xml

then add this to the web.xml

       <servlet-mapping>
		<servlet-name>default</servlet-name>
		<url-pattern>/help/*</url-pattern>
	</servlet-mapping>
</web-app>

In the WebContent folder, create a subfolder called apidocs and create an index.html file in there.

Code your html and javascript
then export as war file and install

Installation:
osgi:install war:file:/Users/foleyc/Downloads/help.war?Web-ContextPath=cityconnect

