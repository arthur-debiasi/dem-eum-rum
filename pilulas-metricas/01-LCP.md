# ⏱️ LCP – Largest Contentful Paint

**O que é:**  
LCP mede o tempo que o **maior elemento principal da página** (imagem, bloco de texto ou vídeo) leva para carregar e aparecer na tela do usuário.

**Elementos que contam como LCP:**  
- Imagens  
- Thumbnails de vídeo  
- Blocos de texto (como títulos e parágrafos)  
- Imagens de fundo (via CSS)  

**Por que é importante:**  
- **Experiência do usuário:** um LCP rápido significa que o conteúdo principal aparece rapidamente, transmitindo sensação de velocidade.  
- **SEO:** Google usa LCP como fator de ranqueamento no Page Experience Update.  
- **Métricas de negócio:** páginas lentas tendem a ter **mais abandono** e **menos conversões**.  

**Meta de mercado:**  
- ✅ Bom: ≤ 2,5s  
- ⚠️ Precisa melhorar: 2,5s – 4s  
- ❌ Ruim: > 4s  

**Como melhorar o LCP:**  
1. **Otimizar recursos:** reduzir tamanho de imagens e outros elementos principais.  
2. **Melhorar TTFB:** reduzir o tempo de resposta do servidor.  
3. **Usar CDN:** distribuir conteúdo mais próximo do usuário.  
4. **Reduzir bloqueios de JS e CSS:** garantir que scripts e estilos não atrasem o LCP.  
5. **Lazy-load de conteúdo abaixo da dobra:** evitar que elementos secundários atrasem o principal.
