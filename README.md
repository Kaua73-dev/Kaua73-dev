<div align="center">

# 👨‍💻 Kauã Santana Jerônimo

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=21&duration=2800&pause=800&color=38D2FF&center=true&vCenter=true&width=820&height=44&lines=Backend+Developer+%2F%2F+Java;Spring+Boot+%C2%B7+Microsservi%C3%A7os+%C2%B7+Docker;TDD%2C+DDD+e+Clean+Code+como+padr%C3%A3o%2C+n%C3%A3o+como+enfeite;Sistemas+que+n%C3%A3o+caem+%C3%A0s+tr%C3%AAs+da+manh%C3%A3" alt="Backend Developer // Java — Spring Boot, microsserviços, Docker. TDD, DDD e Clean Code como padrão, não como enfeite. Sistemas que não caem às três da manhã." />

<img src="./assets/divider.svg" width="100%" alt="" />

<img src="https://komarev.com/ghpvc/?username=Kaua73-dev&style=for-the-badge&color=38D2FF&labelColor=111823&label=VISITAS" alt="Visitas no perfil" />
<img src="https://img.shields.io/github/followers/Kaua73-dev?style=for-the-badge&logo=github&label=SEGUIDORES&color=1B6F9E&labelColor=111823" alt="Seguidores" />

</div>

<img src="./assets/divider.svg" width="100%" alt="" />

## `01` Inicialização

```java
package dev.kaua.core.domain;


public record Desenvolvedor(String name, Nivel nivel, Set<Competencia> stack) {

    public Desenvolvedor {
        Objects.requireNonNull(nome, "nome é obrigatório");
        stack = Set.copyOf(stack);
    }

    public boolean atende(Demanda demanda) {
        return stack.containsAll(demanda.requisitos());
    }

    public Desenvolvedor aprende(Competencia nova) {
        var ampliada = new HashSet<>(stack);
        ampliada.add(nova);
        return new Desenvolvedor(nome, nivel, ampliada);
    }

    // código porco, criado às 2am
}
```

Backend em Java, faço sistema que não quebra de madrugada. 
*Não me chame para codar em php.*
*Não me chame para fazer frontend.*

<img src="./assets/divider.svg" width="100%" alt="" />

## `02` Stack

<div align="center">

<img src="./assets/stack.svg" alt="Stack técnica" width="100%" />

<br><br>

<img src="https://skillicons.dev/icons?i=java,spring,maven,hibernate,nodejs,express,postgres,mysql,mongodb,redis,docker,git,github,linux,postman,idea&theme=dark&perline=8" alt="Ferramentas" />

</div>

<div align="center">

<br><br>

<a href="https://www.linkedin.com/in/kauadevv/">
  <img src="https://img.shields.io/badge/LinkedIn-111823?style=for-the-badge&logo=linkedin&logoColor=38D2FF" alt="LinkedIn" />
</a>
<a href="mailto:kaua.santanaj@gmail.com">
  <img src="https://img.shields.io/badge/Email-111823?style=for-the-badge&logo=gmail&logoColor=38D2FF" alt="Email" />
</a>
<a href="https://github.com/Kaua73-dev">
  <img src="https://img.shields.io/badge/GitHub-111823?style=for-the-badge&logo=github&logoColor=38D2FF" alt="GitHub" />
</a>

<br><br>
</div>
