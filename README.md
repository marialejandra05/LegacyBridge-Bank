# LegacyBridge-Bank
Interface bancária híbrida desenvolvida para integrar processamento Mainframe (COBOL/JCL) com sistemas modernos em Java, focando em arquitetura Batch e processamento de transações.
Este projeto é um estudo de engenharia de software focado na integração de sistemas legados de alta performance com interfaces modernas. O objetivo é simular o ecossistema real de grandes instituições financeiras.

## Tecnologias e Stack
- **Mainframe Layer:** COBOL (Lógica de Negócio), JCL (Controle de Jobs) e VSAM (Armazenamento de Dados).
- **Application Layer:** Java (JDK 17+) para middleware e integração.
- **Tools:** Zowe (opcional para integração Mainframe), Maven/Gradle.

## Arquitetura do Projeto
O sistema opera em um modelo híbrido:
1.  **Processamento Batch:** Arquivos JCL orquestram programas COBOL para processamento de saldos e fechamentos.
2.  **Camada Java:** Atua como a interface de comunicação, enviando e recebendo dados dos arquivos do Mainframe.

##  Estrutura de Pastas
- `/mainframe/cobol`: Fontes dos programas de lógica bancária.
- `/mainframe/jcl`: Scripts de execução e definição de arquivos.
- `/java-app`: Interface e serviços em Java.
- `/docs`: Documentação técnica e diagramas de fluxo.

## Aprendizados Recentes
- [ ] Estrutura de um Job JCL (Cartões JOB, EXEC, DD).
- [ ] Lógica de Divisões no COBOL.
- [ ] Manipulação de arquivos de registros fixos.
