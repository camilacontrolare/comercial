# Landing page: Contabilidade para profissionais da saúde

Página feita para receber os cliques do tráfego pago, com o logo, as cores (laranja e grafite) e o slogan da Controlare.

- `index.html`: a página completa. O logo já está embutido no arquivo, então **basta publicar este arquivo**.
- `logo.png`: cópia do logo, para outros usos.

Conteúdo: formulário de qualificação, soluções, abertura de empresa médica (5 etapas, documentos e prazo de 48h em Juiz de Fora), tabela dos planos Essencial, Gestão e Premium (sem preços, só "a partir de R$ 297/mês"), diferenciais e perguntas frequentes.

## Como funciona

- O formulário (nome, profissão, CNPJ e faturamento) **abre o WhatsApp (32) 98894-9708** com a mensagem já preenchida, e o lead só precisa tocar em "Enviar".
- Se o anúncio usar parâmetros UTM (ex.: `?utm_campaign=medico-pj`), a mensagem chega com `(ref: medico-pj)` no final. Assim a Camila sabe de qual campanha veio o lead e preenche a coluna *Campanha* do pipeline.
- Cada clique em "Falar no WhatsApp" dispara o evento **Lead** do Meta Pixel e do Google, depois que o gestor de tráfego colar os códigos no espaço indicado dentro do `index.html`.

## Como publicar

**Opção 1: no seu site atual (recomendado)**
Na hospedagem do www.contabilidadecontrolare.com.br, crie uma pasta `saude` e envie o `index.html` (pelo painel da hospedagem ou por FTP). A página fica em:
`www.contabilidadecontrolare.com.br/saude`

Se o site for feito em WordPress, Wix ou similar e não aceitar o envio de arquivos, use a opção 2.

**Opção 2: Netlify (grátis, sem programar)**
1. Acesse **app.netlify.com/drop** e crie uma conta.
2. Arraste a pasta `landing-page` para a página.
3. Em segundos sai um link do tipo `controlare-saude.netlify.app`.
4. Opcional: em *Domain settings*, adicione `saude.contabilidadecontrolare.com.br` e crie no seu provedor de domínio o registro DNS que o Netlify indicar.

## Para alterar

- **Cores:** no início do `index.html`, no bloco `:root`.
- **Número do WhatsApp:** variável `WHATSAPP` no final do arquivo.
- **Depoimentos:** quando houver, peça ao Claude para incluir uma seção de depoimentos.
