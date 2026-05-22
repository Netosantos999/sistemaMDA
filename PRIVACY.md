# Política de Privacidade — Sistema MDA Acompanhamento de Obras

**Última atualização:** 22 de maio de 2026  
**Versão do aplicativo:** 4.8  
**Desenvolvedor:** Francelino Neto Santos  
**Contato:** francelinotees@gmail.com

---

## 1. Introdução

O **Sistema MDA Acompanhamento de Obras** ("o Aplicativo") é um software de gestão e controle diário de obras. Esta Política de Privacidade descreve quais informações são coletadas, como são utilizadas e protegidas.

---

## 2. Informações que Coletamos

### 2.1 Informações de Cadastro (Primeiro Acesso)

Para ativar o período de avaliação gratuita, solicitamos:

| Campo | Obrigatoriedade | Finalidade |
|-------|----------------|------------|
| Nome Completo | Obrigatório | Identificação do usuário |
| E-mail | Obrigatório | Comunicação e ativação de licença |
| Telefone / WhatsApp | Opcional | Suporte técnico |
| Empresa ou Obra | Obrigatório | Identificação do contexto de uso |

### 2.2 Identificador de Dispositivo (HWID)

O Aplicativo lê o **GUID de máquina** do registro do Windows (`SOFTWARE\Microsoft\Cryptography\MachineGuid`) para associar sua licença ao dispositivo. Este identificador é anonimizado (hash SHA-256) antes de qualquer armazenamento externo.

### 2.3 Dados do Projeto

Todos os dados inseridos sobre projetos, serviços, logs diários, colaboradores e relatórios são armazenados **exclusivamente no banco de dados local** do seu dispositivo, em:

```
%LOCALAPPDATA%\Sistema MDA\mda.db
```

Esses dados **nunca são enviados para servidores externos** sem o seu consentimento explícito.

---

## 3. Como Utilizamos as Informações

| Dado | Finalidade | Compartilhado com terceiros? |
|------|-----------|------------------------------|
| Nome e E-mail | Gerenciamento de licença (período trial / assinatura) | Somente com o servidor de licenciamento Firebase (Google Cloud) |
| HWID (hash) | Vincular licença ao dispositivo | Somente com o servidor de licenciamento Firebase (Google Cloud) |
| Telefone | Suporte técnico (opcional) | Não |
| Dados do projeto | Funcionamento do sistema | Não — armazenados localmente |

---

## 4. Armazenamento e Segurança

- As informações de cadastro (nome, e-mail) são transmitidas via **HTTPS** para o **Firebase Firestore** (Google Cloud Platform), serviço gerenciado com certificação **SOC 2**, **ISO 27001** e conformidade com o **GDPR**.
- O banco de dados local (`mda.db`) é armazenado no perfil do usuário (`%LOCALAPPDATA%`) e **não pode ser acessado por outros usuários** do mesmo computador.
- O cache de licença local (`.lic`) é protegido com assinatura **HMAC-SHA256** vinculada ao HWID da máquina.

---

## 5. Retenção de Dados

- **Dados de licença no Firebase:** mantidos enquanto a conta estiver ativa. Você pode solicitar a exclusão a qualquer momento pelo e-mail abaixo.
- **Dados do projeto (local):** permanecem no seu dispositivo até você desinstalar o aplicativo ou excluir manualmente.
- **Cache de licença:** expira automaticamente após 30 dias e é renovado com verificação online.

---

## 6. Seus Direitos (LGPD — Lei nº 13.709/2018)

De acordo com a Lei Geral de Proteção de Dados (LGPD), você tem direito a:

- **Acessar** os dados pessoais que temos sobre você
- **Corrigir** informações incorretas
- **Excluir** seus dados pessoais dos nossos servidores
- **Portabilidade** dos seus dados
- **Revogar o consentimento** a qualquer momento

Para exercer qualquer desses direitos, entre em contato:

**E-mail:** francelinotees@gmail.com  
**WhatsApp:** (88) 98813-6586

---

## 7. Serviços de Terceiros

O Aplicativo utiliza os seguintes serviços de terceiros:

| Serviço | Finalidade | Política de Privacidade |
|---------|-----------|------------------------|
| Google Firebase Firestore | Gerenciamento de licenças | [firebase.google.com/support/privacy](https://firebase.google.com/support/privacy) |

---

## 8. Crianças

O Sistema MDA é destinado exclusivamente a uso profissional por adultos. Não coletamos intencionalmente informações de menores de 18 anos.

---

## 9. Alterações nesta Política

Podemos atualizar esta Política de Privacidade periodicamente. Quando houver alterações significativas, notificaremos você através do próprio aplicativo. A data da última atualização está indicada no topo deste documento.

---

## 10. Contato

Para dúvidas, solicitações ou reclamações relacionadas à privacidade:

**Desenvolvedor:** Francelino Neto Santos  
**E-mail:** francelinotees@gmail.com  
**WhatsApp:** (88) 98813-6586  
**Localização:** Brasil

---

*Este documento está em conformidade com a Lei Geral de Proteção de Dados (LGPD — Lei nº 13.709/2018) e com as políticas da Microsoft Store para aplicativos publicados na plataforma Windows.*
