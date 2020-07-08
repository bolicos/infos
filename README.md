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

No Ubuntu basta fazer esse o procedimento abaixo para configurar as tecla (/?°) nos notebooks IMB/Lenovo:

Execute seguinte comando no TERMINAL:

$ sudo dpkg-reconfigure keyboard-configuration

Configure o teclado selecionando as seguintes opções:

Modelo do teclado: IBM ThinkPad R60/R61/T61

País de origem para o teclado: Portuguese (Brazil)

Layout do teclado: Portuguese (Brazil)

Tecla para funcionar como AltGr: O padrão para o layout de teclado

Tecla Compose: Sem tecla compose

Usar Control+Alt+Backspace para terminar o servidor X?: <não>
