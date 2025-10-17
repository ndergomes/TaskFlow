# 🏃 Sprint Planning - TaskFlow

# **🚀 SPRINT 1 - MVP Core (2 semanas)**

## **📦 Setup & Arquitetura**

- [ ] TASK-001: Configurar projeto Vite + React + TypeScript
  - ✅ Verificar se Vite está instalado
  - ✅ Configurar ESLint e Prettier
  - ✅ Criar estrutura de pastas (components, hooks, types, utils)
- [ ] TASK-002: Configurar Tailwind CSS + Radix UI
  - ✅ Instalar Tailwind e configurar tailwind.config.js
  - ✅ Adicionar Radix UI Dialog, Select, Tooltip
  - ✅ Criar tema dark/light com next-themes
- [ ] TASK-003: Configurar Zustand para gerenciamento de estado
  - ✅ Criar store de tarefas (tasks)
  - ✅ Criar store de categorias (categories)
  - ✅ Implementar persist middleware para localStorage

## **🎨 Componentes Base**

- [ ] TASK-004: Criar componente TaskCard
  - ✅ Props: task (objeto), onToggle, onEdit, onDelete
  - ✅ Exibir título, categoria, prioridade
  - ✅ Checkbox para marcar como concluída
  - ✅ Botões de editar e excluir
  - ✅ Animação com Framer Motion ao completar
- [ ] TASK-005: Criar componente TaskModal (adicionar/editar)
  - ✅ Usar Radix Dialog
  - ✅ Formulário com React Hook Form + Zod
  - ✅ Campos: título, descrição, categoria, prioridade
  - ✅ Validação: título obrigatório (min 3 caracteres)
  - ✅ Atalho de teclado Ctrl+N para abrir
  - ✅ Toast de sucesso com Sonner
- [ ] TASK-006: Criar componente TaskList
  - ✅ Renderizar lista de TaskCard
  - ✅ Filtros: categoria, prioridade, status
  - ✅ Ordenação: prioridade, data de criação
  - ✅ Estado vazio com ilustração e CTA
  - ✅ AnimatePresence para animações de lista

## **📱 Página Principal**

- [ ] TASK-007: Criar layout principal (Header + Sidebar + Content)
  - ✅ Header: logo, botão tema, botão adicionar tarefa
  - ✅ Sidebar: filtros e categorias (colapsável no mobile)
  - ✅ Content: TaskList principal
  - ✅ Responsivo: mobile-first
- [ ] TASK-008: Integrar todos os componentes
  - ✅ Conectar TaskModal ao botão de adicionar
  - ✅ Implementar CRUD completo via Zustand
  - ✅ Testar fluxo completo: criar, editar, excluir, filtrar

## **✅ Testes & Refinamento**

- [ ] TASK-009: Testes de usabilidade
  - ✅ Testar em Chrome, Firefox, Safari
  - ✅ Testar em mobile (iOS e Android)
  - ✅ Validar tempo de adição de tarefa (< 15s)
- [ ] TASK-010: Polimento final
  - ✅ Ajustar espaçamentos e cores
  - ✅ Otimizar animações
  - ✅ Adicionar loading states
  - ✅ Revisar acessibilidade (ARIA labels)

# **🚀 SPRINT 2 - Features Avançadas**

- [ ] TASK-011: Implementar PWA (Progressive Web App)
- [ ] TASK-012: Adicionar busca e filtros avançados
- [ ] TASK-013: Dashboard com estatísticas e gráficos
