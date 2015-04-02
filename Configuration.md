# Configuration #
### Basic configuration ###
```
<plugin>
    <groupId>net.mgorski.quicktag</groupId>
    <artifactId>quicktag</artifactId>
    <version>2.1.4</version>
    <executions>
        <execution>
            <phase>generate-sources</phase>
            <goals>
                <goal>quicktag</goal>
            </goals>
        </execution>
    </executions>
    <configuration>
        <outputPackage>com.trainings.spring.basic</outputPackage>
    </configuration>
</plugin>
```
### Additional configuration ###
Inside `configuration` you can use the following:
| **option** | **required** | **default value** | **since** | **description** |
|:-----------|:-------------|:------------------|:----------|:----------------|
|versionClassName|no|Version|? |Name of the generated version file|
|vcs|no|git|1.0.0|Specifies which VCS to use. Available choices: git,svn,hg|
|vcsBinaryPath|no|-|1.0.3|? |Path to the binary of the active VCS. If not set system value is used|
|vcsRepositoryPath|no|-|1.0.3|? |Path to root of repository. If not set root of the project is used|
|outputDirectory|no|${project.basedir}/src/main/java/|1.0.3|Output folder, usually indicates root folder for source files of your project|
|outputPackage|yes|- |1.0.3|Indicates package, where output file should have been generated|
|bambooBuildNumber|no|${bamboo.buildNumber}|? |The Atlassian Bamboo build number|
|bambooBuildTimeStamp|no|${bamboo.buildTimeStamp}|? |The Atlassian Bamboo build timestamp|