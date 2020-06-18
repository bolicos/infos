# infos
Informations

Comandos:
sudo docker run -d --name postgres12 -e POSTGRES_PASSWORD=root -e PGDATA=/var/lib/postgresql/data/pgdata -v /home/cassia/docker/postgres:/var/lib/postgresql/data postgres -h 127.0.0.1


Links:
https://blog.solidsoft.pl/2020/03/02/enable-java-14-preview-features-in-gradle-maven-and-idea/


bootRun {
    doFirst {
        systemProperty "spring.profiles.active", "dev"
    }
}

bootJar {
    archiveFileName = 'assembly.jar'
}

configurations {
    developmentOnly
    runtimeClasspath {
        extendsFrom developmentOnly
    }
}

configurations {
    developmentOnly
    runtimeClasspath {
        extendsFrom developmentOnly
    }
    compileOnly {
        extendsFrom annotationProcessor
    }
}

apply plugin: 'java'

apply plugin: 'idea'

idea {
    module {
        downloadSources = true
    }
}

Install JAVA 14: sudo apt install openjdk-14-jdk -y
sudo update-alternatives  --install /usr/bin/java java /usr/lib/jvm/jdk-14.0.1/bin/java 2082 

@Value("${spring.datasource.username}")
private String username;
ou

@Value("#{environment['spring.datasource.username']}")
private String username;
