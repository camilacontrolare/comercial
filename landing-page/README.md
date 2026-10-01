# Landing page: Contabilidade para profissionais da saúde

Página feita para receber os cliques do tráfego pago, com o logo, as cores (laranja e grafite) e o slogan da Controlare.

- `index.html`: a página completa. O logo já está embutido no arquivo, então **basta publicar este arquivo**.
- `logo.png`: cópia do logo, para outros usos.

Conteúdo: formulário de qualificação, soluções, abertura de empresa médica (5 etapas, documentos e prazo de 48h em Juiz de Fora), tabela dos planos Essencial, Gestão e Premium (sem preços, só "a partir de R$ 297/mês"), diferenciais e perguntas frequentes.

## Como funciona

- O formulário (nome, profissão, CNPJ e faturamento) **abre o WhatsApp (32) 98894-9708** com a mensagem já preenchida, e o lead só precisa tocar em "Enviar".
- Se o anúncio usar parâmetros UTM (ex.: `?utm_campaign=medico-pj`), a mensagem chega com `(ref: medico-pj)` no final. Assim a Camila sabe de qual campanha veio o lead e preenche a coluna *Campanha* do pipeline.
- Cada clique em "Falar no WhatsApp" dispara o evento **Lead** do Meta Pixel e do Google, depois que o gestor de tráfego colar os códigos no espaço indicado dentro do `index.html`.

## Como publicar (site no Wix)

O Wix não aceita o envio de arquivos HTML como página. Por isso a landing page fica hospedada no **Netlify** (grátis) e ganha um endereço do próprio domínio da Controlare: **saude.contabilidadecontrolare.com.br**.

### 1. Publicar no Netlify (5 minutos)
1. No computador, crie uma pasta chamada `controlare-saude` e coloque dentro dela o arquivo `index.html`.
2. Acesse **app.netlify.com/drop** e crie uma conta gratuita (pode entrar com o Google).
3. Arraste a pasta `controlare-saude` para a área indicada na página.
4. Em segundos a página fica no ar, com um endereço do tipo `nome-aleatorio.netlify.app`.
5. Em **Site configuration → Change site name**, troque o nome para algo como `controlare-saude`. O endereço vira `controlare-saude.netlify.app`, que já pode ser usado nos anúncios.

### 2. Usar o domínio da Controlare (opcional, recomendado)
1. No Netlify, abra o site (projeto) e vá em **Domain management** (ou **Project configuration → Domain management**) → **Add a domain** → digite `saude.contabilidadecontrolare.com.br` → confirme.
2. O Netlify vai pedir um registro **CNAME** apontando para `controlare-saude.netlify.app`.
3. Crie esse registro no **Registro.br**, onde o domínio está registrado e o DNS é gerenciado (o site no Wix está conectado por apontamento):
   1. Acesse **registro.br** → **Entrar** e faça login.
   2. Clique no domínio **contabilidadecontrolare.com.br**.
   3. Na seção **DNS**, clique em **Configurar zona DNS** (ou **Editar zona**).
   4. Clique em **Nova entrada** e preencha: Tipo **CNAME**, Nome **saude**, Dados **controlare-saude.netlify.app**.
   5. Clique em **Salvar alterações**. **Não altere os registros que já existem** (eles mantêm o site do Wix no ar).
4. Aguarde a propagação (normalmente minutos, podendo levar até 48 horas). O Netlify ativa o HTTPS (cadeado) automaticamente.

### 3. Ligar ao site atual
No editor do Wix, adicione um botão ou item de menu "Contabilidade para a saúde" com link para `https://saude.contabilidadecontrolare.com.br`.

### Para atualizar a página no futuro
No Netlify, abra o site → **Deploys** → arraste a pasta com o novo `index.html`. O endereço continua o mesmo.

> **Pixel e Google Tag:** os códigos de medição instalados no Wix **não** valem para esta página. O gestor de tráfego precisa colar os códigos no `index.html` (há um espaço indicado no início do arquivo) antes de publicar.

## Para alterar

- **Cores:** no início do `index.html`, no bloco `:root`.
- **Número do WhatsApp:** variável `WHATSAPP` no final do arquivo.
- **Depoimentos:** quando houver, peça ao Claude para incluir uma seção de depoimentos.
