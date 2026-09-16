<div align="center">

<img src="./assets/header.svg" alt="Kauã Santana Jerônimo — Backend Developer" width="100%" />

<br><br>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=21&duration=2800&pause=800&color=38D2FF&center=true&vCenter=true&width=820&height=44&lines=Backend+Developer+%2F%2F+Java;Spring+Boot+%C2%B7+Microsservi%C3%A7os+%C2%B7+Docker;TDD%2C+DDD+e+Clean+Code+como+padr%C3%A3o%2C+n%C3%A3o+como+enfeite;Sistemas+que+n%C3%A3o+caem+%C3%A0s+tr%C3%AAs+da+manh%C3%A3" alt="Backend Developer // Java — Spring Boot, microsserviços, Docker. TDD, DDD e Clean Code como padrão, não como enfeite. Sistemas que não caem às três da manhã." />

<br>

<img src="https://komarev.com/ghpvc/?username=Kaua73-dev&style=for-the-badge&color=38D2FF&labelColor=111823&label=VISITAS" alt="Visitas no perfil" />
<img src="https://img.shields.io/github/followers/Kaua73-dev?style=for-the-badge&logo=github&label=SEGUIDORES&color=1B6F9E&labelColor=111823" alt="Seguidores" />

</div>

<img src="./assets/divider.svg" width="100%" alt="" />

## `01` Inicialização

```java
package dev.kaua.core.domain;

/**
 * A regra de negócio não conhece framework, banco nem HTTP.
 * Se precisa de mock para ser testada, foi modelada errado.
 */
public record Desenvolvedor(String nome, Nivel nivel, Set<Competencia> stack) {

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
}
```

Backend em **Java** e ecossistema **Spring**. Meu trabalho é fazer sistema que continua de pé depois que o tráfego chega.

- **Microsserviços** e **APIs REST** — contrato claro, falha isolada, deploy independente
- **TDD** — teste primeiro, e a suíte roda antes de eu abrir o PR
- **DDD** — domínio no centro, regra de negócio longe do controller
- **Clean Code** e **Design Patterns** — código que o próximo dev entende sem me chamar
- **SQL e NoSQL** — modelagem, índice e query que não degrada quando a tabela cresce
- **Docker** e **Git** — ambiente reproduzível, histórico legível
- **Node.js** quando o problema pede, sem trocar de religião por isso

<img src="./assets/divider.svg" width="100%" alt="" />

## `02` Stack

<div align="center">

<img src="./assets/stack.svg" alt="Stack técnica" width="100%" />

<br><br>

<img src="https://skillicons.dev/icons?i=java,spring,maven,hibernate,nodejs,express,postgres,mysql,mongodb,redis,docker,git,github,linux,postman,idea&theme=dark&perline=8" alt="Ferramentas" />

</div>

<img src="./assets/divider.svg" width="100%" alt="" />

## `03` Telemetria

<div align="center">

<img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Kaua73-dev&theme=github_dark" alt="Linguagens por repositório" />
<img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Kaua73-dev&theme=github_dark" alt="Linguagens por commit" />

<br>

<img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Kaua73-dev&theme=github_dark" alt="Estatísticas gerais" />
<img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=Kaua73-dev&theme=github_dark&utcOffset=-3" alt="Horários de commit" />

<br><br>

<img src="https://streak-stats.demolab.com?user=Kaua73-dev&hide_border=true&background=111823&border=233246&stroke=233246&ring=38D2FF&fire=38D2FF&currStreakNum=E6EDF3&currStreakLabel=38D2FF&sideNums=E6EDF3&sideLabels=8FA3B8&dates=5E7285" alt="Sequência de commits" />

</div>

<img src="./assets/divider.svg" width="100%" alt="" />

## `04` Canal aberto

<div align="center">

<a href="https://www.linkedin.com/in/kau%C3%A3-santana-jer%C3%B4nimo-611a1a292/">
  <img src="https://img.shields.io/badge/LinkedIn-111823?style=for-the-badge&logo=linkedin&logoColor=38D2FF" alt="LinkedIn" />
</a>
<a href="mailto:kaua.santanaj@gmail.com">
  <img src="https://img.shields.io/badge/Email-111823?style=for-the-badge&logo=gmail&logoColor=38D2FF" alt="Email" />
</a>
<a href="https://github.com/Kaua73-dev">
  <img src="https://img.shields.io/badge/GitHub-111823?style=for-the-badge&logo=github&logoColor=38D2FF" alt="GitHub" />
</a>

<br><br>

<img src="./assets/divider.svg" width="100%" alt="" />

<sub>Aberto a oportunidades e a código que sobrevive ao próximo sprint.</sub>

</div>
