# ⚙️ Configuração e Personalização - Do Café ao Casamento

## 📋 Checklist de Personalização Pré-Deploy

### ✅ Informações de Contato
Substitua os seguintes placeholders pelos dados reais da empresa:

```html
<!-- TELEFONE/WHATSAPP -->
Localizar: (11) 99999-9999
Substituir por: Número real da empresa
Arquivos afetados: index.html (múltiplas ocorrências)

<!-- EMAIL CORPORATIVO -->
Localizar: contato@docafeaocasamento.com.br  
Substituir por: Email real da empresa
Arquivos afetados: index.html

<!-- ENDEREÇO -->
Localizar: São Paulo, SP - Atendemos toda a Grande São Paulo
Substituir por: Endereço específico da empresa
Arquivos afetados: index.html

<!-- HORÁRIOS DE FUNCIONAMENTO -->
Localizar: Segunda a Sexta: 9h às 18h | Sábado: 9h às 15h
Substituir por: Horários reais de atendimento
Arquivos afetados: index.html
```

### 📱 Links de Redes Sociais
```html
<!-- INSTAGRAM -->
Localizar: https://instagram.com/docafeaocasamento
Substituir por: URL real do Instagram da empresa

<!-- FACEBOOK -->
Localizar: https://facebook.com/docafeaocasamento  
Substituir por: URL real do Facebook da empresa

<!-- WHATSAPP LINKS -->
Localizar: https://wa.me/5511999999999
Substituir por: https://wa.me/55[código_área][número_real]
```

### 🎨 Branding Personalizado

#### Logo da Empresa
```html
<!-- LOGO PLACEHOLDER ATUAL -->
<div class="w-10 h-10 bg-gradient-to-br from-gold-500 to-gold-600 rounded-full flex items-center justify-center">
    <i class="fas fa-coffee text-white text-lg"></i>
</div>

<!-- SUBSTITUIR POR -->
<img src="assets/logo.png" alt="Do Café ao Casamento" class="h-10 w-auto">
```

#### Favicon
Criar e adicionar no `<head>`:
```html
<link rel="icon" type="image/png" sizes="32x32" href="assets/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="assets/favicon-16x16.png">
<link rel="apple-touch-icon" sizes="180x180" href="assets/apple-touch-icon.png">
```

## 🖼️ Substituição de Imagens

### Imagens Prioritárias para Substituição
```javascript
// HERO SECTION - Imagem principal
Atual: 'https://images.unsplash.com/photo-1519225421980-715cb0215aed'
Novo: 'assets/images/hero-evento-principal.jpg'
Dimensões: 1920x1080px (16:9)

// SOBRE NÓS - Equipe
Atual: 'https://images.unsplash.com/photo-1556909114-f6e7ad7d3136'  
Novo: 'assets/images/equipe-profissional.jpg'
Dimensões: 1000x600px

// GALERIA - Substituir todas as 6 imagens
assets/images/gallery/cafe-manhã-1.jpg
assets/images/gallery/churrasco-gourmet-1.jpg
assets/images/gallery/festa-15anos-1.jpg
assets/images/gallery/evento-corporativo-1.jpg
assets/images/gallery/casamento-luxuoso-1.jpg
assets/images/gallery/cafe-manhã-2.jpg
Dimensões: 1000x800px cada

// DEPOIMENTOS - Fotos de clientes reais
assets/images/clients/cliente-1.jpg (Maria Silva)
assets/images/clients/cliente-2.jpg (Carlos Santos)  
assets/images/clients/cliente-3.jpg (Ana Costa)
Dimensões: 100x100px (quadradas)

// BLOG - Imagens dos artigos
assets/images/blog/festa-junina-decoracao.jpg
assets/images/blog/cafe-manhã-sofisticado.jpg
assets/images/blog/tendencias-casamento-2024.jpg
Dimensões: 1000x600px (16:10)
```

### Estrutura de Pastas Recomendada
```
assets/
├── images/
│   ├── hero/
│   │   └── evento-principal.jpg
│   ├── gallery/
│   │   ├── cafe-manhã-1.jpg
│   │   ├── churrasco-gourmet-1.jpg
│   │   └── [outras imagens]
│   ├── services/
│   │   ├── cafe-da-manha.jpg
│   │   ├── churrasco-gourmet.jpg
│   │   └── [outras imagens]
│   ├── clients/
│   │   └── [fotos de depoimentos]
│   ├── blog/
│   │   └── [imagens dos artigos]
│   └── team/
│       └── equipe-profissional.jpg
├── icons/
│   ├── favicon-32x32.png
│   ├── favicon-16x16.png
│   └── apple-touch-icon.png
└── logo/
    ├── logo.png
    ├── logo-white.png
    └── logo.svg
```

## 💰 Personalização de Orçamentos

### Faixas de Preço (Ajustar conforme mercado local)
```html
<!-- FORMULÁRIO DE ORÇAMENTO -->
<option value="ate-5k">Até R$ 5.000</option>
<option value="5k-10k">R$ 5.000 - R$ 10.000</option>
<option value="10k-20k">R$ 10.000 - R$ 20.000</option>
<option value="20k-50k">R$ 20.000 - R$ 50.000</option>
<option value="acima-50k">Acima de R$ 50.000</option>

<!-- AJUSTAR CONFORME REALIDADE LOCAL -->
<!-- Exemplo para mercado de menor poder aquisitivo: -->
<option value="ate-2k">Até R$ 2.000</option>
<option value="2k-5k">R$ 2.000 - R$ 5.000</option>
<!-- Ou para mercado premium: -->
<option value="10k-25k">R$ 10.000 - R$ 25.000</option>
<option value="25k-50k">R$ 25.000 - R$ 50.000</option>
```

## 🎯 SEO Personalizado

### Meta Tags por Localização
```html
<!-- PERSONALIZAR CIDADE/REGIÃO -->
<title>Do Café ao Casamento - Eventos Luxuosos em [SUA_CIDADE]</title>
<meta name="description" content="Planejamento de eventos luxuosos em casa em [SUA_CIDADE] - do café da manhã ao casamento. Serviços premium de catering e organização de festas personalizadas.">
<meta name="keywords" content="festas em casa [SUA_CIDADE], organização de 15 anos [SUA_CIDADE], eventos luxuosos, catering premium, planejamento de casamento">

<!-- STRUCTURED DATA - ADICIONAR ENDEREÇO REAL -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "EventPlanner", 
  "name": "Do Café ao Casamento",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "[ENDEREÇO_COMPLETO]",
    "addressLocality": "[CIDADE]",
    "addressRegion": "[ESTADO]", 
    "postalCode": "[CEP]",
    "addressCountry": "BR"
  },
  "telephone": "[TELEFONE_REAL]",
  "url": "[URL_DO_SITE]"
}
</script>
```

## 📊 Analytics e Tracking

### Google Analytics 4
```html
<!-- ADICIONAR ANTES DO </head> -->
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### Facebook Pixel
```html
<!-- FACEBOOK PIXEL -->
<script>
!function(f,b,e,v,n,t,s)
{if(f.fbq)return;n=f.fbq=function(){n.callMethod?
n.callMethod.apply(n,arguments):n.queue.push(arguments)};
if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
n.queue=[];t=b.createElement(e);t.async=!0;
t.src=v;s=b.getElementsByTagName(e)[0];
s.parentNode.insertBefore(t,s)}(window,document,'script',
'https://connect.facebook.net/en_US/fbevents.js');
fbq('init', 'YOUR_PIXEL_ID_HERE');
fbq('track', 'PageView');
</script>
```

### Eventos de Conversão
```javascript
// ADICIONAR AOS BOTÕES E FORMULÁRIOS
// WhatsApp Click
onClick="gtag('event', 'whatsapp_click', { 'event_category': 'contact' });"

// Formulário Enviado  
onSubmit="gtag('event', 'form_submit', { 'event_category': 'lead' });"

// Quiz Completo
onClick="gtag('event', 'quiz_complete', { 'event_category': 'engagement' });"

// Serviço Visualizado
onClick="gtag('event', 'service_view', { 'event_category': 'interest', 'service_type': 'casamento' });"
```

## 🔧 Integrações Técnicas

### Formulário com Backend Real
```javascript
// SUBSTITUIR SIMULAÇÃO POR INTEGRAÇÃO REAL
// Exemplo com Netlify Forms:
<form name="contact" method="POST" data-netlify="true">

// Exemplo com Formspree:
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">

// Exemplo com EmailJS:
// Implementar JavaScript real para envio via EmailJS
```

### WhatsApp API (Opcional)
```javascript
// INTEGRAÇÃO MAIS AVANÇADA COM WHATSAPP BUSINESS API
function sendWhatsAppMessage(phone, message) {
    // Implementar integração real com WhatsApp Business API
    // Ou usar serviços como Twilio, ChatAPI, etc.
}
```

## 🌐 Configurações de Hosting

### Netlify (Recomendado)
```toml
# netlify.toml
[build]
  command = "echo 'No build needed'"
  publish = "."

[[redirects]]
  from = "/*"
  to = "/index.html"
  status = 200

[headers]
  for = "/*"
  [headers.values]
    X-Frame-Options = "DENY"
    X-XSS-Protection = "1; mode=block"
```

### Vercel
```json
// vercel.json
{
  "rewrites": [
    { "source": "/(.*)", "destination": "/index.html" }
  ],
  "headers": [
    {
      "source": "/(.*)",
      "headers": [
        { "key": "X-Frame-Options", "value": "DENY" },
        { "key": "X-XSS-Protection", "value": "1; mode=block" }
      ]
    }
  ]
}
```

## 📧 Email Marketing

### Lista de Captura
```html
<!-- ADICIONAR CAMPOS OPCIONAIS PARA NEWSLETTER -->
<div class="mt-4">
    <label class="flex items-center">
        <input type="checkbox" name="newsletter" class="mr-2">
        <span class="text-sm text-navy-600">Quero receber dicas de eventos por email</span>
    </label>
</div>
```

### Integração com Mailchimp/RD Station
```javascript
// EXEMPLO DE INTEGRAÇÃO
function subscribeNewsletter(email, name) {
    // Implementar API call para plataforma escolhida
    fetch('https://api.mailchimp.com/3.0/lists/LIST_ID/members', {
        method: 'POST',
        headers: {
            'Authorization': 'Bearer YOUR_API_KEY',
            'Content-Type': 'application/json'
        },
        body: JSON.stringify({
            email_address: email,
            status: 'subscribed',
            merge_fields: {
                FNAME: name
            }
        })
    });
}
```

## 🔒 Segurança

### Headers de Segurança
```nginx
# Para servidores Nginx
add_header X-Frame-Options "SAMEORIGIN" always;
add_header X-XSS-Protection "1; mode=block" always;
add_header X-Content-Type-Options "nosniff" always;
add_header Referrer-Policy "no-referrer-when-downgrade" always;
add_header Content-Security-Policy "default-src 'self' http: https: data: blob: 'unsafe-inline'" always;
```

### SSL/HTTPS
- Certificado SSL obrigatório
- Redirect HTTP para HTTPS
- HSTS headers configurados

---

## 📝 Checklist Final Pré-Launch

- [ ] Todas as informações de contato atualizadas
- [ ] Imagens placeholder substituídas por fotos reais
- [ ] Logo profissional implementado
- [ ] Favicon configurado
- [ ] Google Analytics configurado
- [ ] Facebook Pixel implementado (se aplicável)
- [ ] Formulários testados e funcionando
- [ ] WhatsApp links funcionando corretamente
- [ ] SEO meta tags personalizadas
- [ ] Sitemap.xml gerado
- [ ] Robots.txt configurado
- [ ] SSL certificado ativo
- [ ] Performance testada (PageSpeed Insights)
- [ ] Responsividade testada em dispositivos reais
- [ ] Cross-browser testing completo
- [ ] Backup dos arquivos realizados

*Seguir este checklist garante um launch profissional e sem problemas técnicos.*