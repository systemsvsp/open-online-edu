# Open Online Education Collaboration and Learning Environment (OOEDU LMS)

This is the source code for the OOEdu.

The master branch is the most current development release, 21.
The other branches are currently or previously supported releases. See below for more information on the release plan and support schedule.

## Building

To build Sakai you need Java 1.8. Once you have clone a copy of this repository you can
build it by running (or `./mvnw install` if you don't have Maven installed):
```
mvn install
```

## Running

OOEdu runs on Apache Tomcat 9. Download the latest version from http://tomcat.apache.org and extract the archive.
*Note: Sakai does not work with Tomcat installed via a package from apt-get, yum or other package managers.*

When you are done, deploy Sakai to Tomcat:
```
mvn clean install sakai:deploy -Dmaven.tomcat.home=/path/to/your/tomcat
```

Now start Tomcat:
```
cd /path/to/your/tomcat/bin
./startup.sh && tail -f ../logs.catalina.out
```

Once Sakai has started up (it usually takes around 30 seconds), open your browser and navigate to http://localhost:8080/portal

## Licensing

OoEdu is licensed under the [Educational Community License version 2.0](http://opensource.org/licenses/ECL-2.0) 

OoEdu is an Open Online Education project and follows the Foundation's guidelines and requirements for ECL-2.0.

## Contributing

See [our dedicated page](CONTRIBUTING.md) for more information on contributing to OoEdu.

## Get in touch
If you have any questions, please join the Sakai developer mailing list: To subscribe send an email to systemsvsp@gmail.com

If you want more immediate response during M-F typical business hours you could try our Slack channels.

If you can't find your  "at institution.edu" on the OOEdu signup page then send an email requesting access for yourself and your institution 

## Community supported versions

## Under Development

## Skinning OOEdu
Documentation on how to alter the OOEdu skin (look and feel) is here https://github.com/systemsvsp/open-online-edu.

## Translating OOEdu

Translation, internationalization and localization of the OOEdu project are coordinated by the OOEdu Internationalization/localization community. 

From its inception, the OOEdu project has been envisioned and designed for global use. Complete or majority-complete translations of Sakai are available in the languages listed below. 

### Supported languages
| Locale | Language|
| ------ | ------ |
| en_US | English (Default) |
| ca_ES | Catalán |
| es_ES | Español |
| eu | Euskera |
| fa_IR | Farsi |
| fr_FR | Français |
| hi_IN | Hindi |
| ja_JP | Japanese |
| mn | Mongolian |
| pt_BR | Portuguese (Brazil) |
| sv_SE | Swedish |
| tr_TR | Turkish |
| zh_CN | Chinese |
| ar | Arabic |

### Other languages

Other languages can be used depends on the usage.
