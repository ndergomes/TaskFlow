# 📚 Documentação Técnica - TaskFlow

# **🏛️ Arquitetura do Sistema**

## **Stack Tecnológico**

- Frontend: React 18 + TypeScript + Vite
- Styling: Tailwind CSS + Radix UI
- State: Zustand com persist middleware
- Forms: React Hook Form + Zod
- Animation: Framer Motion
- Icons: Lucide React
- Notifications: Sonner

## **Estrutura de Pastas**

src/

- components/ - Componentes reutilizáveis
  - TaskCard.tsx
  - TaskModal.tsx
  - TaskList.tsx
  - Header.tsx
  - Sidebar.tsx
- store/ - Zustand stores
  - taskStore.ts
  - categoryStore.ts
- types/ - TypeScript types
  - task.ts
  - category.ts
- hooks/ - Custom hooks
  - useKeyboardShortcut.ts
  - useTaskFilters.ts
- utils/ - Funções utilitárias
  - cn.ts - Class name merger
  - date.ts - Date formatters

## **Modelo de Dados**

Task Interface:

- id: string (UUID)
- title: string (obrigatório, min 3 chars)
- description: string (opcional)
- categoryId: string
- priority: 'high' | 'medium' | 'low'
- completed: boolean
- createdAt: Date
- updatedAt: Date

Category Interface:

- id: string (UUID)
- name: string
- color: string (hex)
- icon: string (Lucide icon name)

# **🎨 Padrões de Design**

## **Tema & Cores**

- Dark mode como padrão
- Paleta: Slate + Cyan para acentos
- Prioridades: Red (alta), Amber (média), Green (baixa)
- Usar next-themes para toggle dark/light

## **Animações**

- Fade + Scale para modais (duration: 200ms)
- Slide para lista de tarefas (stagger: 50ms)
- Pulse suave ao completar tarefa
- Usar AnimatePresence para exit animations

## **Responsividade**

- Mobile-first approach
- Breakpoints: sm (640px), md (768px), lg (1024px)
- Sidebar colapsável em mobile
- Touch-friendly: min 44px para botões

# **✅ Critérios de Aceitação**

- [ ] Adicionar tarefa em < 15 segundos
- [ ] Funciona em Chrome, Firefox, Safari
- [ ] Responsivo em mobile (iOS e Android)
- [ ] Persistência de dados via localStorage
- [ ] Acessibilidade: ARIA labels, navegação por teclado
- [ ] Loading states e feedback visual
- [ ] Sem erros no console

# **🛠️ Comandos Úteis**

- npm run dev - Iniciar servidor de desenvolvimento
- npm run build - Build de produção
- npm run lint - Verificar erros de linting
- npm run preview - Preview do build
