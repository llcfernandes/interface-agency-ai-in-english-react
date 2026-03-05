# agency.ai — Digital Agency Landing Page

> Modern, animated and fully responsive digital agency landing page built with React 19, Tailwind CSS v4 and Framer Motion.

![React](https://img.shields.io/badge/React-19-61DAFB?style=flat&logo=react) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-v4-06B6D4?style=flat&logo=tailwindcss) ![Framer Motion](https://img.shields.io/badge/Framer_Motion-12-EF0084?style=flat&logo=framer) ![Vite](https://img.shields.io/badge/Vite-7-646CFF?style=flat&logo=vite)

## Overview

**agency.ai** is a front-end personal project designed to simulate a real digital agency product page. The focus was on delivering a polished UI experience with micro-interactions, scroll-triggered animations, and a consistent design system across light and dark modes. The entire interface was built from scratch using isolated React components, Tailwind CSS v4 and Framer Motion for animation orchestration.

## Tech Stack

| Technology | Version | Role |
|---|---|---|
| React | 19.2.0 | UI component architecture |
| Tailwind CSS | 4.1.18 | Utility-first styling & dark mode |
| Framer Motion | 12.34.3 | Scroll animations & transitions |
| Vite | 7.3.1 | Build tool & dev server |
| Web3Forms | API | Contact form submission backend |
| React Hot Toast | 2.6.0 | Toast notification system |
| Manrope | Google Fonts | Primary typeface |

## Notable Implementation Details

**Custom Animated Cursor** — The default cursor is hidden via CSS. A two-layer custom cursor is implemented in `App.jsx` using `useRef` refs: a solid dot that snaps to the exact mouse position, and an outline ring that follows with a lerp smoothing effect driven by `requestAnimationFrame`.

**Mouse-Tracking Spotlight** — Each `ServiceCard` listens to `onMouseMove` and calculates the cursor position relative to the card using `getBoundingClientRect`, dynamically positioning a radial gradient behind the content to create a real-time glow effect.

**Theme System** — Theme state lives in `App.jsx`, initialized from `localStorage`. `ThemeToggleBtn` detects system preference via `window.matchMedia` on first load, toggling the `dark` class on `<html>` to activate Tailwind's dark variant — defined with `@custom-variant` in `index.css`.

**Animation Strategy** — All sections use Framer Motion's `whileInView` with `viewport={{ once: true }}` and `staggerChildren` for orchestrated, one-time entrance animations as the user scrolls.

## Author

Developed by **Lucas Fernandes** — [Link](https://interface-agenci-ai-in-english-react-qr6kj9wtd.vercel.app)

---

# agency.ai — Landing Page de Agência Digital

> Landing page moderna, animada e totalmente responsiva para agência digital, construída com React 19, Tailwind CSS v4 e Framer Motion.

![React](https://img.shields.io/badge/React-19-61DAFB?style=flat&logo=react) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-v4-06B6D4?style=flat&logo=tailwindcss) ![Framer Motion](https://img.shields.io/badge/Framer_Motion-12-EF0084?style=flat&logo=framer) ![Vite](https://img.shields.io/badge/Vite-7-646CFF?style=flat&logo=vite)

## Visão Geral

**agency.ai** é um projeto pessoal de front-end criado para simular a página de produto real de uma agência digital. O foco foi entregar uma experiência de UI bem acabada com micro-interações, animações ativadas pelo scroll e um sistema de design consistente nos modos claro e escuro. Toda a interface foi construída do zero com componentes React isolados, Tailwind CSS v4 e Framer Motion para orquestração das animações.

## Stack Tecnológica

| Tecnologia | Versão | Função |
|---|---|---|
| React | 19.2.0 | Arquitetura de componentes UI |
| Tailwind CSS | 4.1.18 | Estilização utilitária e modo escuro |
| Framer Motion | 12.34.3 | Animações de scroll e transições |
| Vite | 7.3.1 | Build tool e servidor de desenvolvimento |
| Web3Forms | API | Backend para envio do formulário de contato |
| React Hot Toast | 2.6.0 | Sistema de notificações toast |
| Manrope | Google Fonts | Tipografia principal |

## Detalhes Técnicos Relevantes

**Cursor Animado Personalizado** — O cursor padrão é ocultado via CSS. Um cursor em duas camadas é implementado no `App.jsx` usando refs: um ponto sólido que acompanha exatamente o mouse, e um anel externo com efeito de suavização lerp conduzido por `requestAnimationFrame`.

**Spotlight no Hover** — Cada `ServiceCard` escuta o `onMouseMove` e calcula a posição do cursor via `getBoundingClientRect`, posicionando dinamicamente um gradiente radial atrás do conteúdo para criar um efeito de brilho em tempo real.

**Sistema de Tema** — O estado do tema vive no `App.jsx`, inicializado pelo `localStorage`. O `ThemeToggleBtn` detecta preferência do sistema via `window.matchMedia` e aplica o tema alternando a classe `dark` no `<html>`, ativando a variante dark do Tailwind — definida com `@custom-variant` no `index.css`.

**Estratégia de Animação** — Todas as seções usam `whileInView` com `viewport={{ once: true }}` e `staggerChildren` para animações de entrada orquestradas e disparadas uma única vez no scroll.

## Autor

Desenvolvido por **Lucas Fernandes** — [Link](https://interface-agenci-ai-in-english-react-qr6kj9wtd.vercel.app)
