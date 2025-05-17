# Abra: Chatbot de Apoio Emocional

**Abra** é um chatbot desenvolvido em Python com o objetivo de fornecer apoio emocional e descontração aos usuários. Utilizando a tecnologia de inteligência artificial generativa do Google Gemini, o Abra é capaz de compreender as emoções expressas no texto do usuário e responder de maneira amigável, atenciosa e acolhedora.

---

## Índice

1. [Descrição](#descrição)
2. [Funcionalidades Principais](#funcionalidades-principais)
3. [Instalação](#instalação)
4. [Uso](#uso)
5. [Configuração](#configuração)
6. [Intenções Reconhecidas](#intenções-reconhecidas)
7. [Personalidade do Chatbot](#personalidade-do-chatbot)
8. [Intervenção em Crise](#intervenção-em-crise)
9. [Contribuindo](#contribuindo)

---

## Descrição

O Abra foi projetado com uma personalidade jovem e informal, criando um ambiente seguro e de suporte. Suas principais funcionalidades incluem:

* Identificação de diferentes intenções emocionais.
* Prática de escuta ativa e validação dos sentimentos do usuário.
* Intervenção em situações de crise, indicando recursos de ajuda profissional (CVV, CAPS).

---

## Funcionalidades Principais

1. **Identificação de Intenções**
   Reconhece diversos contextos emocionais, como ansiedade, solidão, desmotivação, medo do futuro, pressão acadêmica, entre outros.

2. **Personalidade Amigável**
   Persona jovem (16–24 anos), linguagem informal, uso moderado de gírias e emojis.

3. **Apoio Emocional**
   Escuta ativa, validação de sentimentos e incentivo.

4. **Intervenção em Crise**
   Em casos de isolamento extremo ou menção de autoagressão, oferece localização para indicar serviços como CVV (188) e CAPS.

5. **Geração de Respostas com IA**
   Integração com o Google Gemini para produzir respostas contextuais.

6. **Fluxos de Conversação**
   Exercícios de respiração, dicas para solidão, pressão acadêmica etc.

7. **Base de Dados de Recursos**
   Contatos básicos de CVV e CAPS para algumas regiões.

8. **Modo Interativo**
   Interface via terminal de linha de comando.

---

## Instalação

### Pré-requisitos

* Python 3.x
* Chave da API do Google Cloud (para usar o modelo Gemini).

### 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/abra-chatbot.git
cd abra-chatbot
```

### 2. Instalar dependências

```bash
pip install google-generativeai IPython
```

---

## Uso

1. Defina sua chave de API do Google:

   * No Google Colab, adicione um *Secret* chamado `GOOGLE_API_KEY`.
   * Localmente, exporte como variável de ambiente:

     ```bash
     export GOOGLE_API_KEY="sua_chave_aqui"
     ```

2. Execute o chatbot:

   ```bash
   python abra.py
   ```

3. O Abra irá iniciar no terminal e solicitará seu nome. A partir daí, basta conversar!

---

## Configuração

* **GOOGLE\_API\_KEY**
  Necessária para IA generativa. Pode ser definida em *Secrets* (Colab) ou variável de ambiente.

* **Outros Ambientes**
  Se não usar Colab, ajuste a forma de carregamento da chave no código.

---

## Intenções Reconhecidas

| Intenção               | Exemplo de palavras-chave                    |
| ---------------------- | -------------------------------------------- |
| ansiedade              | "ansiedade", "pânico"                        |
| solidão                | "sozinho", "isolado"                         |
| desmotivação           | "sem ânimo", "desmotivado"                   |
| medo\_futuro           | "não sei o que farei", "futuro me assusta"   |
| pressao\_academica     | "excesso de tarefas", "estou sobrecarregado" |
| dificuldade\_adaptacao | "difícil me adaptar", "não me sinto parte"   |
| problema\_social       | "não tenho amigos", "me sinto deslocado"     |
| saudacao               | "oi", "olá"                                  |
| agradecimento          | "obrigado", "valeu"                          |
| despedida              | "tchau", "até logo"                          |
| informacao\_recursos   | "onde encontro ajuda", "número do CVV"       |
| padrao                 | quaisquer mensagens sem correspondência      |

---

## Personalidade do Chatbot

* **Nome:** Abra
* **Idade aparente:** 16–24 anos
* **Tom:** Empático, acolhedor, descontraído (com seriedade)
* **Linguagem:** Informal, respeitosa, uso moderado de gírias e emojis
* **Foco:** Escuta ativa, validação de sentimentos e incentivo
* **Evitar:** Diagnósticos médicos, aconselhamento legal, linguagem robótica ou excessivamente técnica

---

## Intervenção em Crise

Ao identificar menções de autoagressão ou isolamento extremo, o Abra pergunta, de forma respeitosa:

> “Você poderia me informar sua cidade e estado? Assim posso indicar serviços de apoio próximos, como CAPS e o CVV (188).”

---

## Contribuindo

Contribuições são bem-vindas! Para colaborar:

1. Faça um *fork* do projeto.
2. Crie uma branch com sua feature:

   ```bash
   git checkout -b minha-nova-feature
   ```
3. Faça commit das suas alterações:

   ```bash
   git commit -m "Adicionar nova funcionalidade X"
   ```
4. Envie para o repositório remoto:

   ```bash
   git push origin minha-nova-feature
   ```
5. Abra um Pull Request.

---

> Desenvolvido com ❤️ para promover bem-estar e suporte emocional.
