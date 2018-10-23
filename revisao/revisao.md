## Revisão GCES

### Padrões relacionados a manutenção de Software
- IEEE 1219
- ISO/IEC [ISO95]

### Tipos de Manutenção
- Manutenção Corretiva: Reparo de erros.
- Manutenção Adaptativa: Adaptação do software às mudanças no ambiente.
- Manutenção de Aperfeiçoamento (Perfectiva): Implementação de novas funcionalidades a partir de novos requisitos, melhorias de perfomance e melhoria de usabilidade.
- Manutenção Preventiva: Melhore na manutenabilidade do sistema, melhorias na documentação, modularização e estrutura do sistema. Detcção e correção de potenciais erros.

### Leis de Lehman
1. Mudanças Contínuas (Continuing change)
2. Aumento na Complexidade (Increasing complexity)
3. Crescimento Contínua (Continuing growth)
4. Declínio da Qualidade (Declining quality)

### Conceitos GCS
- Baselines: Pontos de referência para o desenvolvimento.
- Itens de Configuração: Todo e qualquer item que faz parte do baseline e do projeto (código, imagem, documentação e etc).
- Configuração de Software: A junção desses e demais itens relacionados ao desenvolvimento de um software, além da configuração e manutenção dos mesmos (estado dos itens, estado do software).
- Responsabilidades:
	- Controle de Versão: Definição de Versão, Baselines.
	- Controle de Mudanças: Porque e o foi mudado, quem mudou e ferramentas.
	- Auditoria das Configurações:
		- Física: checa se aconteceu
		- Funcional: aconteceu de forma correta?
		- Reportar Descobertas

### Controle de Versão
Sistema de Controle de Versão (VCS)
- Mantém registrado
	- O que foi alterado
	- Quando foi alterado
	- Quem alterou
	- Porque alterou
- Histórico de mudanças
- Permite voltar e avançar nas modificações
	- Ver diferentes estados
	- Desfazer mudanças
- Previnem perda de informações
- Comparação de estados
	- Ajuda em resolução de bugs

- Políticas de Compartilhamento
	- Cópia de Trabalho
	- Trava-Modifica-Destrava
	- Copia-Modifica-Resolve

- Repositório
	Guarda arquivos, configurações e todas as versões dos itens de configuração.

### Integração Contínua
Na engenharia de software, a integração contínua é a prática de mesclar todas as cópias de trabalho do desenvolvedor em uma linha principal compartilhada várias vezes ao dia.

- Benefícios e Boas Práticas
	1. Build Automática
	2. Build Testável
	3. Commits diários na master
	4. Commits testados e funcionando na master
	5. Build Rápida
	6. Deploy Automático

- Deploy Contínuo: Entrega contínua em produção ao cliente.
- Entrega Contínuo (Continuous Delivery): A habilidade de gerar uma build estável a qualquer momento.

### Automação de Build
- Automação das tarefas/passos
- Geração de diferentes Builds
	- Desenvolvimento
	- Produção
	- Teste
- Utiliza os dados corretos para cada ambiente
	- Senha
	- Banco
	- Acessos a APIs

### Licenças de Software
Classificação das Licenças

- Recíprocas Totais (_Copyleft_): O software é livre, deve permanecer livre e trabalhos derivados devem ser também livres (AGPL, GPL e Similares).
- Recíprocas Parciais (_Copyleft_ fraco): O software é livre e deve permanecer livre, mas trabalhos derivados não precisam ser livres (LGPL, EPL, MPL e assemelhadas).
- Permissivas: O software é livre, mas pode ser relicenciado sem permissão adicional do autor (Apache, MIT/X11, BSD e assemelhadas).

Software Livre: 4 Liberdades
1. Usar
2. Copiar
3. Contribuir (fazer trabalhos derivados)
4. (Re)distribuir