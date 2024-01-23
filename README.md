To test the Plugin, follow instructions to copy plugin to the project
https://docs.craftercms.org/en/4.1/by-role/developer/composable/extensions/resources/form-control-plugins.html

Append below to after rte control in site-config-tools.xml
(Location (In Repository) SITENAME/config/studio/administration/site-config-tools.xml)

                  <control>
                    <plugin>
                        <pluginId>org.craftercms.plugin.excontrol</pluginId>
                        <type>control</type>
                        <name>link</name>
                        <filename>main.js</filename>
                    </plugin>
                    <icon>
                        <class>fa-link</class>
                    </icon>
                </control>


Data Sources must be setup before Link Plugin can function as expected. e.g.

1. File Browse
   Title: Page Source
   Browse Path: /site/website/
2. File Broswe
   Title: File Source
   Browse Path: /static-assets/
