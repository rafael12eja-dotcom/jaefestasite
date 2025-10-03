# 🎨 Guia de Estilo - Do Café ao Casamento

## Paleta de Cores

### Cores Principais
```css
/* Ouro - Cor principal da marca */
--gold-100: #FEF7E0  /* Fundo suave */
--gold-300: #F5E6A3  /* Hover states */  
--gold-500: #D4AF37  /* Cor primária */
--gold-600: #B8941F  /* Bordas e ícones */
--gold-700: #9C7C10  /* Estados ativos */

/* Marfim - Fundo neutro elegante */
--ivory-100: #FFFEF9  /* Fundo principal */
--ivory-200: #FAF9F0  /* Fundo secundário */
--ivory-300: #F5F4E8  /* Divisores suaves */

/* Blush - Accent romântico */
--blush-100: #FCF1F1  /* Fundo suave */
--blush-300: #F7D7D7  /* Elementos decorativos */
--blush-500: #E8B4B8  /* Cor de destaque */
--blush-600: #D49499  /* Bordas e ícones */

/* Navy - Texto principal */
--navy-500: #1E293B  /* Texto corpo */
--navy-600: #0F172A  /* Títulos */
--navy-700: #020617  /* Texto enfático */

/* Esmeralda - Accent nature */
--emerald-500: #10B981  /* Cor de sucesso */
--emerald-600: #059669  /* Hover success */
--emerald-700: #047857  /* Active success */
```

### Gradientes Assinatura
```css
/* Gradiente principal da marca */
.gradient-primary {
  background: linear-gradient(135deg, #D4AF37, #E8B4B8, #10B981);
}

/* Gradiente para botões */
.gradient-button {
  background: linear-gradient(135deg, #D4AF37, #B8941F);
}

/* Gradiente para hero background */
.gradient-hero {
  background: linear-gradient(135deg, rgba(212, 175, 55, 0.1) 0%, rgba(232, 180, 184, 0.1) 50%, rgba(16, 185, 129, 0.1) 100%);
}
```

## Tipografia

### Hierarquia de Fontes
```css
/* Títulos elegantes */
font-family: 'Playfair Display', serif;
/* Uso: H1, H2, H3, Logo, Citações especiais */

/* Interface moderna */
font-family: 'Montserrat', sans-serif;  
/* Uso: Navegação, botões, labels, UI elements */

/* Texto corpo legível */
font-family: 'Crimson Text', serif;
/* Uso: Parágrafos, descrições, conteúdo extenso */
```

### Tamanhos e Pesos
```css
/* Títulos */
.text-5xl { font-size: 3rem; }      /* H1 - Hero */
.text-4xl { font-size: 2.25rem; }   /* H2 - Seções */
.text-3xl { font-size: 1.875rem; }  /* H3 - Subsections */
.text-2xl { font-size: 1.5rem; }    /* H4 - Cards */
.text-xl  { font-size: 1.25rem; }   /* H5 - Pequenos títulos */

/* Corpo */
.text-lg  { font-size: 1.125rem; }  /* Texto principal */
.text-base{ font-size: 1rem; }      /* Texto padrão */
.text-sm  { font-size: 0.875rem; }  /* Texto secundário */
.text-xs  { font-size: 0.75rem; }   /* Labels e hints */

/* Pesos */
.font-light    { font-weight: 300; }
.font-normal   { font-weight: 400; }
.font-medium   { font-weight: 500; }
.font-semibold { font-weight: 600; }
.font-bold     { font-weight: 700; }
```

## Componentes

### Botões
```css
/* Botão primário luxuoso */
.btn-luxury {
  background: linear-gradient(135deg, #D4AF37, #B8941F);
  color: white;
  padding: 1rem 2rem;
  border-radius: 9999px;
  font-weight: 600;
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.btn-luxury:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 25px rgba(212, 175, 55, 0.3);
}

/* Botão secundário */
.btn-secondary {
  background: rgba(255, 254, 249, 0.15);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
  color: white;
}
```

### Cards de Serviço
```css
.service-card {
  background: white;
  border-radius: 1rem;
  padding: 2rem;
  box-shadow: 0 20px 40px rgba(212, 175, 55, 0.15), 0 10px 20px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.service-card:hover {
  transform: translateY(-10px) scale(1.02);
}
```

### Efeitos Visuais
```css
/* Sombra luxuosa */
.luxury-shadow {
  box-shadow: 0 20px 40px rgba(212, 175, 55, 0.15), 0 10px 20px rgba(0, 0, 0, 0.1);
}

/* Efeito glass */
.glass-effect {
  background: rgba(255, 254, 249, 0.15);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
}

/* Texto gradiente */
.text-gradient {
  background: linear-gradient(135deg, #D4AF37, #E8B4B8, #10B981);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
```

## Animações

### Keyframes Personalizados
```css
@keyframes fadeIn {
  0% { opacity: 0; transform: translateY(20px); }
  100% { opacity: 1; transform: translateY(0); }
}

@keyframes slideUp {
  0% { opacity: 0; transform: translateY(50px); }
  100% { opacity: 1; transform: translateY(0); }
}

@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-10px); }
}

@keyframes parallax {
  0% { transform: translateY(0px); }
  100% { transform: translateY(-50px); }
}
```

### Classes de Animação
```css
.animate-fade-in { animation: fadeIn 1s ease-in-out; }
.animate-slide-up { animation: slideUp 0.8s ease-out; }
.animate-float { animation: float 6s ease-in-out infinite; }
.animate-parallax { animation: parallax 20s linear infinite; }
```

## Responsividade

### Breakpoints
```css
/* Mobile First Approach */
/* xs: 0px - 639px (default) */
/* sm: 640px+ */
/* md: 768px+ */  
/* lg: 1024px+ */
/* xl: 1280px+ */
/* 2xl: 1536px+ */
```

### Padrões Responsivos
```css
/* Container responsivo */
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1.5rem;
}

/* Grid responsivo */
.grid-responsive {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
}

@media (min-width: 768px) {
  .grid-responsive {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 1024px) {
  .grid-responsive {
    grid-template-columns: repeat(3, 1fr);
  }
}
```

## Elementos Brasileiros

### Padrões Sutis
```css
/* Padrão tropical discreto */
.tropical-pattern {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='40' height='40' viewBox='0 0 40 40'%3E%3Cg fill='%23d4af37' fill-opacity='0.03'%3E%3Cpath d='M20 20c0-11.046-8.954-20-20-20v20h20zm20 0c0-11.046-8.954-20-20-20v20h20z'/%3E%3C/g%3E%3C/svg%3E");
}
```

### Cores com Referência Cultural
- **Ouro**: Riqueza natural do Brasil, elegância
- **Esmeralda**: Exuberância da natureza brasileira  
- **Blush**: Calor humano, acolhimento
- **Navy**: Sofisticação internacional

## Iconografia

### Font Awesome Icons Utilizados
```html
<!-- Serviços -->
<i class="fas fa-coffee"></i>        <!-- Café -->
<i class="fas fa-fire"></i>          <!-- Churrasco -->
<i class="fas fa-crown"></i>         <!-- 15 Anos -->
<i class="fas fa-briefcase"></i>     <!-- Corporativo -->
<i class="fas fa-mask"></i>          <!-- Temático -->
<i class="fas fa-ring"></i>          <!-- Casamento -->

<!-- Contato -->
<i class="fab fa-whatsapp"></i>      <!-- WhatsApp -->
<i class="fas fa-envelope"></i>      <!-- Email -->
<i class="fas fa-map-marker-alt"></i><!-- Local -->
<i class="fas fa-clock"></i>         <!-- Horário -->

<!-- Navegação -->
<i class="fas fa-bars"></i>          <!-- Menu -->
<i class="fas fa-times"></i>         <!-- Fechar -->
<i class="fas fa-chevron-down"></i>  <!-- Scroll -->
<i class="fas fa-arrow-right"></i>   <!-- Próximo -->
```

## Uso de Imagens

### Diretrizes para Fotos
1. **Qualidade**: Mínimo 1920x1080px para hero images
2. **Estilo**: Fotografia profissional, bem iluminada
3. **Cores**: Harmonizar com a paleta da marca
4. **Composição**: Regra dos terços, elementos balanceados
5. **Formato**: WebP preferencial, fallback JPEG

### Proporções Recomendadas
- **Hero**: 16:9 (landscape)
- **Service Cards**: 4:3 (mais quadrado)
- **Gallery**: Variado (masonry layout)
- **Blog Thumbnails**: 16:9
- **Testimonial Photos**: 1:1 (circular)

## Acessibilidade

### Contraste de Cores
- **Texto em Gold (#D4AF37)**: Usar apenas em fundos escuros
- **Texto em Navy (#1E293B)**: Contraste AAA em fundos claros
- **Links**: Sempre com hover states visíveis
- **Botões**: Estados de foco claramente definidos

### Navegação
- **Tab Order**: Lógico e intuitivo
- **Skip Links**: Para conteúdo principal
- **Alt Text**: Todas as imagens descritas
- **ARIA Labels**: Elementos interativos identificados

---

*Este guia deve ser seguido para manter a consistência visual e a experiência de marca premium em todas as futuras atualizações do website.*