# 🧠 Mapa Mental de Monitoramento de Experiência do Usuário

## Tipos Principais

### 1. RUM (Real User Monitoring)
- **Dados:** Usuários reais
- **Foco:** Performance técnica e erros
- **Perfil recomendado:** Dev / Gerente
- **Métricas típicas:**
  - LCP (Largest Contentful Paint)
  - FID (First Input Delay)
  - CLS (Cumulative Layout Shift)
  - FCP (First Contentful Paint)
  - TTFB (Time To First Byte)
  - Taxa de erros JS
  - Taxa de crash

### 2. EUM (End User Monitoring)
- **Dados:** Usuários reais
- **Foco:** Experiência percebida, engajamento
- **Perfil recomendado:** Gerente / Dev (insights estratégicos)
- **Métricas típicas:**
  - Duração média da sessão
  - Page Views / sessão
  - Bounce Rate / abandono
  - Funil de conversão
  - Caminhos percorridos (user flow)
  - Disponibilidade / Uptime

### 3. DEM (Digital Experience Monitoring)
- **Dados:** Múltiplas fontes (RUM + EUM + infraestrutura)
- **Foco:** Visão holística da experiência digital
- **Perfil recomendado:** DevOps / Gerente
- **Métricas típicas:**
  - Todas métricas RUM + EUM
  - Latência de rede
  - Performance de servidores e APIs externas
  - SLA / SLO

### 4. Synthetic Monitoring
- **Dados:** Fluxos simulados
- **Foco:** Disponibilidade e performance preventiva
- **Perfil recomendado:** Dev / Ops
- **Métricas típicas:**
  - Tempo de resposta de páginas e APIs
  - Disponibilidade de endpoints
  - Alertas de erro

### 5. Session Replay
- **Dados:** Sessões reais
- **Foco:** UX detalhado
- **Perfil recomendado:** UX / Dev
- **Métricas típicas:**
  - Cliques, scrolls, movimentos do mouse
  - Identificação de pontos de frustração

### 6. Core Web Vitals
- **Dados:** RUM / Google
- **Foco:** Performance percebida
- **Perfil recomendado:** Dev front-end / Produto / SEO
- **Métricas típicas:**
  - LCP, FID, CLS, FCP


# 📘 Manual de Métricas de RUM / EUM

## 1. RUM – Real User Monitoring

### Performance de Carregamento
- **LCP (Largest Contentful Paint):** tempo até o maior conteúdo visível ser carregado
- **FID (First Input Delay):** tempo entre primeira interação e resposta
- **CLS (Cumulative Layout Shift):** instabilidade visual da página
- **FCP (First Contentful Paint):** tempo até aparecer o primeiro conteúdo
- **TTFB (Time To First Byte):** latência do servidor

### Experiência de Sessão
- Tempo médio de carregamento por página
- Tempo de resposta de APIs / endpoints
- Taxa de erros JavaScript

### Confiabilidade / Estabilidade
- Taxa de crash
- Taxa de erro HTTP (4xx, 5xx)
- Erros por versão / deploy

**Perfil recomendado:** Desenvolvedores (foco em otimização técnica), Gerentes (impacto real em usuários)


## 2. EUM – End User Monitoring

### Experiência do Usuário e Engajamento
- Duração média da sessão
- Page Views / sessão
- Bounce Rate / taxa de abandono
- Funil de conversão
- Caminhos percorridos (user flow)

### Confiabilidade Resumida
- Disponibilidade / Uptime
- Erros críticos x número de usuários afetados

### Dimensão Contextual
- Localização geográfica
- Dispositivo / Browser / OS
- Tipo de rede (Wi-Fi, 4G, 5G, fibra)
- Versão do App / Front-end

**Perfil recomendado:** Gerentes / PMs (foco em UX, conversão, retenção), Desenvolvedores (insights estratégicos sobre impacto)


## 3. Métricas Híbridas (RUM + EUM)
- **Apdex Score:** satisfação agregada baseada em thresholds de tempo
- **Tempo médio de carregamento:** diagnóstico técnico e percepção do usuário
- **Taxa de crash / erros:** impacto técnico e de negócio
