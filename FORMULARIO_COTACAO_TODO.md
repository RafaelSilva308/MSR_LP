# Formulário de Cotação — A implementar

Seção: `#contact` (atualmente só tem botões de telefone e WhatsApp)

## Campos do formulário (retirados da página antiga)

| Campo                        | Tipo     | Obrigatório |
|------------------------------|----------|-------------|
| Nome                         | text     | Sim         |
| Sobrenome                    | text     | Sim         |
| CPF / CNPJ                   | text     | Não         |
| E-mail                       | email    | Sim         |
| Telefone / WhatsApp          | tel      | Sim         |
| Origem: Cidade/UF            | text     | Sim         |
| Destino: Cidade/UF           | text     | Sim         |
| Volume                       | text     | Sim         |
| Comprimento (cm)             | number   | Sim         |
| Largura (cm)                 | number   | Sim         |
| Altura (cm)                  | number   | Sim         |
| Peso (kg)                    | number   | Sim         |
| Valor NF (R$)                | text     | Não         |
| Detalhes / Observações       | textarea | Não         |

## Opções de backend

- **WhatsApp** — montar `wa.me/559132363888?text=...` com os campos codificados (mais simples, sem servidor)
- **E-mail via EmailJS** — serviço gratuito que envia do browser sem backend
- **Formspree / Web3Forms** — POST direto para serviço externo, retorna JSON
- **Backend próprio** — Node/PHP recebe e envia e-mail via SMTP

## Estilo sugerido

Manter o fundo escuro vermelho/laranja da seção `#contact` atual e adicionar o formulário abaixo dos botões de telefone/WhatsApp, ou criar uma nova seção antes do CTA final.
