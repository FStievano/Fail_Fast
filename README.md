# Projeto CI/CD - Fail Fast

Este projeto demonstra uma pipeline de automação utilizando GitHub Actions.

## Estrutura da Pipeline

A pipeline possui dois Jobs:

1. Validação do Código
2. Simulação de Build

## Dependência entre Jobs

O Job de build só executa se o Job de validação for concluído com sucesso.

## Uso de Secrets

A pipeline lê um valor secreto configurado no GitHub e exibe uma mensagem no log.

## Conceito de Fail Fast

Caso o primeiro Job falhe, o segundo Job não será executado, garantindo que erros sejam detectados rapidamente.