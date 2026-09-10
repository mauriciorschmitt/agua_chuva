# Calculadora de aproveitamento de água de chuva

Calculadora aberta de potencial de captação de água de chuva em coberturas, conforme ABNT NBR 15527:2019. Estudo de caso: Universidade do Contestado, Campus Mafra (SC).

Arquivo único, sem dependências de build. Os cálculos rodam inteiramente no navegador e nenhum dado é enviado a servidor.

## Publicar no GitHub Pages

1. Crie um repositório público, por exemplo `agua-chuva-unc`.
2. Envie o `index.html` para a raiz do repositório. Pela interface web: **Add file › Upload files**, arraste o arquivo, **Commit changes**.
3. Vá em **Settings › Pages**.
4. Em *Source*, escolha **Deploy from a branch**. Em *Branch*, selecione `main` e a pasta `/ (root)`. Salve.
5. Em um ou dois minutos o endereço aparece na mesma tela, no formato `https://SEU-USUARIO.github.io/agua-chuva-unc/`.

O arquivo precisa se chamar `index.html` e estar na raiz, senão a página não abre no endereço curto.

Pelo terminal, se preferir:

```bash
git init
git add index.html README.md
git commit -m "Calculadora de aproveitamento de água de chuva"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/agua-chuva-unc.git
git push -u origin main
```

Depois é só ativar o Pages em Settings › Pages, como nos passos 3 a 5.

## Como usar

Todos os parâmetros ficam na coluna da esquerda e nos campos abaixo das barras de chuva. Qualquer alteração recalcula a página inteira na hora.

O botão **Copiar link com estes valores** gera um endereço que embute todos os parâmetros. Serve para mandar um cenário específico por e-mail ou deixar preparado antes de uma apresentação. O botão **Imprimir** gera uma versão limpa em PDF pelo diálogo do navegador.

## O que ainda precisa ser substituído

| Parâmetro | Onde buscar |
|---|---|
| Precipitação mensal | Normais Climatológicas 1991–2020 do INMET, estações Mafra, Rio Negro, Rio Negrinho ou Canoinhas. Séries diárias no BDMEP. |
| Chuva de projeto (i) | Equação IDF de Mafra. Software Plúvio da UFV, ou *Chuvas Intensas no Brasil*, de Pfafstetter. |
| Tarifa | Conta de água do campus. Confirmar a categoria tarifária junto ao SIMAE de Mafra e Rio Negro. |
| População do campus | Secretaria acadêmica e RH. |
| Custos de implantação | Cotação local de reservatório e orçamento de projeto hidráulico. |
| Área pavimentada | Medição em imagem de satélite, junto com as coberturas. |

## Normas aplicadas

- **NBR 15527:2019** — aproveitamento de coberturas em áreas urbanas para fins não potáveis
- **NBR 10844:1989** — instalações prediais de águas pluviais
- **NBR 5626** — exige separação total entre a rede de água de chuva e a rede de água potável

## Licença

Livre para copiar, adaptar e usar em outras instituições.
