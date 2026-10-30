# Igor | Suporte de TI · Linux · Desenvolvimento

Estudante de Análise e Desenvolvimento de Sistemas e estagiário de suporte de TI no Pará.
Busco estágio ou vaga júnior em **suporte (N1/N2) ou infraestrutura**, sem deixar de programar.

Meu critério para saber se um sistema está bom: ele continua funcionando quando a luz acaba?
Gosto de entender como as pessoas trabalham, achar a causa real do problema e só dizer que
funciona depois de testar.

**Contato:** igorlira491@gmail.com

---

## Projetos

### Sistema de registro para biblioteca pública · [ver código](https://github.com/igorlira491-debug/sistema-biblioteca)

**O problema:** registrar o uso de 28 computadores em um local sem internet garantida,
com quedas de energia frequentes e dados pessoais de crianças.

- Funciona **100% offline** em uma única máquina, com servidor em Python sem dependências externas
- **Não perde dados em queda de energia**: testado matando o processo (`kill -9`) durante as gravações
- **Dados pessoais cifrados** no navegador (AES-GCM, PBKDF2), seguindo a LGPD
- Backup automático diário, relatórios em PDF e gráficos para a gestão
- **149 verificações de teste**, incluindo recuperação após queda, segurança e desempenho

`Python` `SQLite` `JavaScript` `Web Crypto API`

<img src="https://raw.githubusercontent.com/igorlira491-debug/sistema-biblioteca/main/capturas/tela-geral.png" alt="Painel do sistema da biblioteca, com o mapa dos 28 computadores e dados fictícios" width="600">

### App Android para clínica de terapia infantil · código privado

**O problema:** a rotina da clínica estava espalhada entre sistema, planilha, papel e
WhatsApp, e tarefas como confirmar sessões e remarcar faltas eram esquecidas.

- Tela que mostra **o que precisa ser feito hoje**, com lembretes que funcionam mesmo com o app fechado
- Requisitos levantados com quem usa, a partir de conversas, fotos e vídeo do trabalho real
- Segurança em primeiro lugar: **banco cifrado, PIN por pessoa, backup cifrado e registro de ações**
- Funciona offline, com migração testada entre versões do banco de dados
- **Mais de 180 testes no computador e mais de 100 em celular real**

`Kotlin` `Jetpack Compose` `Room` `SQLCipher`

*Em fase de testes com a cliente, usando dados fictícios. O código é privado para proteger a cliente.*

---

## Um problema que investiguei

**O notebook que congelava sem explicação.** Ele travou quatro vezes, quase sem deixar rastro.
Na quarta, os logs do kernel finalmente mostraram um erro em loop no driver de vídeo (`amdgpu`).
Ajustei um parâmetro do kernel, conferi depois de reiniciar que ele estava ativo e agora estou
observando se o problema voltou.

## O que eu uso

**Linux e suporte:** Linux Mint pelo terminal, `systemd`, `journalctl`, `dmesg`, permissões,
`cron`, diagnóstico de hardware, gráficos e áudio, backup com `rsync`

**Segurança defensiva:** UFW, análise de portas e serviços com `ss`, verificação de integridade
com `sha256sum`, cifragem de dados

**Desenvolvimento:** Python, JavaScript, HTML, CSS, Kotlin, Vue 3, C, SQLite, Git

## Como eu trabalho

- **Testo antes de dizer que funciona**, inclusive simulando falhas
- **Sei lidar com o público:** aprendi atendimento e negociação trabalhando no comércio local
- **Registro decisões** para que outra pessoa consiga continuar o trabalho
- **Uso IA (Claude Code) como ferramenta de desenvolvimento** e assumo a responsabilidade pelo
  que entrego: requisitos, decisões de segurança, testes e aprovação de cada etapa

## Formação

- **Análise e Desenvolvimento de Sistemas**, UNAMA (conclusão prevista: dezembro de 2027)
- **Gestão de Ameaças em Cibersegurança**, SENAC Pará (2026)
