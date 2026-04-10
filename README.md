# uti-vasoativos-calc

Calculadora clínica de drogas vasoativas para uso em Unidade de Terapia Intensiva Adulto.

---

## Sobre o projeto

Ferramenta desenvolvida com base em 10 anos de atuação em UTI Adulto de alta complexidade. O objetivo é centralizar, em uma interface objetiva, os cálculos de velocidade de infusão das principais drogas vasoativas utilizadas na rotina intensivista — eliminando etapas manuais sujeitas a erro em situações de instabilidade hemodinâmica.

Não substitui protocolo institucional nem prescrição médica. Funciona como apoio ao raciocínio clínico durante o preparo e a conferência de infusões.

---

## Drogas disponíveis

| Droga | Classe | Unidade |
|---|---|---|
| Noradrenalina | Vasopressor | mcg/kg/min |
| Dopamina | Vasopressor / Inotrópico | mcg/kg/min |
| Dobutamina | Inotrópico | mcg/kg/min |
| Vasopressina | Vasopressor | UI/h |
| Adrenalina | Vasopressor / Inotrópico | mcg/kg/min |
| Nitroprussiato | Vasodilatador | mcg/kg/min |

---

## Funcionalidades

- Cálculo de velocidade de infusão em mL/h a partir de peso, dose e diluição
- Tabela de concentrações para as principais diluições padronizadas de cada droga
- Indicador visual de posição na faixa terapêutica (habitual / elevada / crítica)
- Informações farmacológicas: mecanismo de ação, indicação, cuidados de enfermagem
- Interface responsiva para uso em tablet e desktop à beira-leito

---

## Como usar

Aplicação estática — sem dependências de backend, sem instalação.

```bash
# Clonar o repositório
git clone https://github.com/SnDann/uti-vasoativos-calc.git

# Abrir diretamente no navegador
open index.html
```

Ou acessar via deploy: [link Vercel]

---

## Cálculo aplicado

**Drogas em mcg/kg/min:**

```
Velocidade (mL/h) = dose (mcg/kg/min) x peso (kg) x 60
                    ─────────────────────────────────────
                         concentração (mcg/mL)

Concentração (mcg/mL) = mg_total x 1000 / volume (mL)
```

**Vasopressina (UI/h):**

```
Velocidade (mL/h) = dose (UI/min) x 60
                    ──────────────────
                    concentração (UI/mL)
```

---

## Referências clínicas

- Protocolo de Choque Séptico — Surviving Sepsis Campaign 2021
- Manual de Drogas Vasoativas em UTI — AMIB
- Bulas dos fabricantes consultadas para apresentação e concentrações

---

## Autor

**Daniel Pereira da Cruz Junior**
Técnico de Enfermagem — UTI Adulto — COREN-SP Ativo
10 anos de atuação em terapia intensiva adulta de alta complexidade

LinkedIn: [linkedin.com/in/sndanndev](https://linkedin.com/in/sndanndev)
GitHub: [github.com/SnDann](https://github.com/SnDann)

---

## Aviso

Este projeto tem finalidade educacional e de apoio técnico. Toda administração de droga vasoativa deve seguir protocolo institucional vigente e prescrição médica. Validar sempre com a equipe assistente antes de qualquer alteração de conduta.
