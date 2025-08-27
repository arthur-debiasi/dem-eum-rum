# 🧠 Guia Didático de Monitoramento da Experiência do Usuário

Monitorar a experiência dos usuários é essencial para entender tanto a performance técnica de um sistema quanto a percepção real de quem o utiliza. Existem diferentes abordagens, cada uma com foco, perfil de uso e métricas próprias. Vamos detalhar.

---

## 1. RUM – Real User Monitoring

O RUM coleta dados diretamente de usuários reais enquanto eles usam o sistema. Seu foco é performance técnica e erros, oferecendo insights precisos para desenvolvedores e gerentes que querem entender como o sistema se comporta “no mundo real”.

**Métricas principais:**

- **LCP (Largest Contentful Paint):** mede quanto tempo leva para o maior elemento visível da página carregar. Um LCP alto indica que o usuário está esperando muito para ver conteúdo importante.
- **FID (First Input Delay):** avalia a velocidade da primeira interação. Se o usuário clica em um botão, quanto tempo o sistema leva para responder?
- **CLS (Cumulative Layout Shift):** monitora instabilidades visuais, como elementos que “pulam” na tela.
- **FCP (First Contentful Paint)** e **TTFB (Time To First Byte):** medem quando o primeiro conteúdo aparece e a latência do servidor, respectivamente.
- **Taxa de erros JavaScript e crashes:** indicam problemas que podem quebrar a experiência.

💡 **Para quem:** Desenvolvedores e gerentes que querem agir sobre performance e estabilidade.

---

## 2. EUM – End User Monitoring

O EUM também coleta dados de usuários reais, mas com foco em experiência percebida e engajamento. É útil para gestores e PMs que desejam entender comportamento, conversão e satisfação.

**Métricas principais:**

- **Duração média da sessão** e **Page Views por sessão:** mostram quanto tempo e quantas páginas os usuários visitam.
- **Bounce Rate / abandono:** indica quantos usuários saem sem interagir.
- **Funil de conversão e caminhos percorridos:** revelam como os usuários navegam e onde eles podem estar travando.
- **Disponibilidade / Uptime:** mesmo sem olhar performance técnica detalhada, garante que os usuários estão conseguindo acessar o sistema.

💡 **Contexto adicional:** EUM pode segmentar por localização, dispositivo, browser, rede e versão do app, ajudando a entender diferenças na experiência entre grupos de usuários.

---

## 3. Métricas Híbridas e DEM

Quando combinamos RUM e EUM com dados de infraestrutura, entramos no campo do Digital Experience Monitoring (DEM). Ele oferece uma visão holística, contemplando performance, engajamento e confiabilidade do sistema.

**Métricas típicas:**

- Todas as métricas de RUM e EUM
- Latência de rede e performance de APIs externas
- SLA / SLO para acompanhar acordos de serviço
- Apdex Score: um índice que sintetiza satisfação dos usuários com base em tempos de resposta
- Taxa de crash e erros: combinando impacto técnico e de negócio

💡 **Para quem:** DevOps e gerentes que precisam de uma visão completa do impacto no usuário e na operação.

---

## 4. Synthetic Monitoring

Aqui, os fluxos são simulados, permitindo testar disponibilidade e performance antes que o usuário real seja impactado. Métricas típicas incluem tempo de resposta de páginas e APIs, disponibilidade de endpoints e alertas de erro. É ideal para equipes de desenvolvimento e operação que querem prevenir problemas.

---

## 5. Session Replay

Essa abordagem grava sessões reais, permitindo assistir a interação do usuário com o sistema. É excelente para identificar frustrações e gargalos de UX: cliques, scrolls, movimentos do mouse e pontos onde o usuário trava.

💡 **Para quem:** UX designers e desenvolvedores que querem insights detalhados de comportamento real.

---

## 6. Core Web Vitals

Definido pelo Google, foca na percepção de performance do usuário. Mede LCP, FID, CLS e FCP, ajudando a priorizar otimizações no front-end que realmente impactam a experiência percebida.

💡 **Para quem:** Desenvolvedores front-end, equipe de produto e SEO.

---
