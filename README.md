<div align="center">

<img alt="Fernando Figueiredo — análise de dados e business intelligence" src="assets/hero.svg" width="100%">

<a href="https://www.linkedin.com/in/fernandofigueiredoalves/">
  <img alt="pergunta, evidência, decisão — análise de dados com SQL, Power BI, Python e machine learning" src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&pause=1200&duration=3600&color=00E5FF&center=true&vCenter=true&width=720&height=44&lines=pergunta+%E2%86%92+evid%C3%AAncia+%E2%86%92+decis%C3%A3o;an%C3%A1lise+de+dados+orientada+a+decis%C3%A3o+de+neg%C3%B3cio;SQL+%C2%B7+Power+BI+%C2%B7+Python+%C2%B7+Machine+Learning;10%2B+anos+em+Comunica%C3%A7%C3%A3o%2C+Estrat%C3%A9gia+e+Storytelling">
</a>

**Analista de Dados | Data Analyst** | SQL · Python · Business Intelligence (BI) | IA & Machine Learning | Data Storytelling | 10+ anos em Comunicação Estratégica<br>
Aberto a vagas de Análise de Dados (incluindo júnior) e posições de entrada em Data Science

<img alt="SQL" src="https://img.shields.io/badge/SQL-151C2B?style=flat-square&labelColor=151C2B">
<img alt="Power BI" src="https://img.shields.io/badge/Power%20BI-151C2B?style=flat-square&logo=powerbi&logoColor=A970FF">
<img alt="Python" src="https://img.shields.io/badge/Python-151C2B?style=flat-square&logo=python&logoColor=A970FF">
<img alt="Machine Learning" src="https://img.shields.io/badge/Machine%20Learning-151C2B?style=flat-square&logo=scikitlearn&logoColor=A970FF">

</div>

---

## `$ python -i bio.py`

```python
"""Bio executável"""

from collections.abc import Iterable
from dataclasses import dataclass

import pandas as pd


@dataclass(frozen=True)
class Perfil:
    nome: str
    base: str
    competencias: tuple[str, ...]
    stack: tuple[str, ...]
    foco: tuple[str, ...]


fernando = Perfil(
    nome="Fernando Figueiredo",
    base="10+ anos em Comunicação, Estratégia de Conteúdo e Storytelling",
    competencias=(
        "Análise de Dados",
        "Pensamento Analítico",
        "Comunicação Estratégica",
    ),
    stack=("SQL", "Power BI", "Python", "Machine Learning"),
    foco=(
        "Analista de Dados",
        "Data Analytics",
        "Business Intelligence Analyst",
        "Product Analyst",
        "Marketing Analytics",
    ),
)

# Repertório em formato longo: um domínio, uma habilidade por linha.
repertorio = pd.DataFrame(
    {
        "dominio": ["Comunicação", "Comunicação", "Dados", "Dados"],
        "habilidade": ["narrativa", "estratégia", "análise", "machine learning"],
    }
)


def bloco(titulo: str, corpo: str) -> None:
    print(f"\n\n{titulo}")
    print(corpo)


def espacado(itens: Iterable[str]) -> str:
    return "\n\n".join(itens)


def bio(p: Perfil, repertorio: pd.DataFrame) -> None:
    leitura = repertorio.groupby("dominio", sort=False)["habilidade"].agg(" · ".join)

    print(f"\n{p.nome.upper()}")
    print("=" * 64)

    bloco("BASE", f"  {p.base}")
    bloco("COMPETÊNCIAS", f"  {' · '.join(p.competencias)}")
    bloco("STACK", f"  {' · '.join(p.stack)}")
    bloco("FOCO", espacado(f"  → {cargo}" for cargo in p.foco))
    bloco(
        "LEITURA DOS DADOS",
        "\n" + espacado(f"  {dominio:<14} {hab}" for dominio, hab in leitura.items()),
    )
    bloco(
        "HIPÓTESE",
        espacado(
            (
                "  Comunicação + narrativa + pensamento analítico",
                "  = capacidade de transformar informação em entendimento.",
            )
        ),
    )
    bloco("OUTPUT", "  transformar dados em respostas.")


if __name__ == "__main__":
    bio(fernando, repertorio)
```

<details>
<summary><b>saída</b></summary>

```text
FERNANDO FIGUEIREDO
================================================================


BASE
  10+ anos em Comunicação, Estratégia de Conteúdo e Storytelling


COMPETÊNCIAS
  Análise de Dados · Pensamento Analítico · Comunicação Estratégica


STACK
  SQL · Power BI · Python · Machine Learning


FOCO
  → Analista de Dados

  → Data Analytics

  → Business Intelligence Analyst

  → Product Analyst

  → Marketing Analytics


LEITURA DOS DADOS

  Comunicação    narrativa · estratégia

  Dados          análise · machine learning


HIPÓTESE
  Comunicação + narrativa + pensamento analítico

  = capacidade de transformar informação em entendimento.


OUTPUT
  transformar dados em respostas.
```

</details>

---

## `$ cat formacao.md`

**Formação técnica em dados**

| Área | Formação | Instituição |
|---|---|---|
| Python | Curso completo de Python | Curso em Vídeo — Gustavo Guanabara |
| SQL | CS50's Databases with SQL | Harvard University |
| Power BI | Microsoft Certified: Power BI Data Analyst Associate | Microsoft |
| Análise de Dados | Formação Analista de Dados | Asimov Academy |
| Machine Learning | Machine Learning Specialization | DeepLearning.AI · Stanford University |

---

## `$ contact --list`

```console
email     fernandofigueiredo123@gmail.com
linkedin  in/fernandofigueiredoalves
```

[**LinkedIn**](https://www.linkedin.com/in/fernandofigueiredoalves/) · [**E-mail**](mailto:fernandofigueiredo123@gmail.com)

<!--
  TRACK B — seção de métricas do GitHub.
  Descomentar somente quando as três condições estiverem satisfeitas:
    1. os commits estiverem sendo contabilizados no grafo de contribuições;
    2. "Include private contributions on my profile" estiver ligado nas configurações;
    3. existirem ao menos dois repositórios públicos.
  Antes disso, estes cartões exibem zeros.

---

## `$ git log --stat`

<div align="center">
<img alt="Estatísticas do GitHub de Fernando Figueiredo" src="https://github-readme-stats.vercel.app/api?username=fernandofigueiredo2201&show_icons=true&hide=stars,issues&hide_border=true&bg_color=00000000&title_color=00E5FF&icon_color=A970FF&text_color=AAB8CC">
<img alt="Gráfico de atividade de contribuições" src="https://github-readme-activity-graph.vercel.app/graph?username=fernandofigueiredo2201&hide_border=true&bg_color=00000000&color=AAB8CC&line=00E5FF&point=A970FF&area=true">
<img alt="Animação da cobra percorrendo o gráfico de contribuições" src="https://raw.githubusercontent.com/fernandofigueiredo2201/fernandofigueiredo2201/output/snake-dark.svg">
</div>
-->
