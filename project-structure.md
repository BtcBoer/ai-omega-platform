# AI Omega Platform - Project Structure

```
ai-omega-platform/
├── .github/                      # GitHub Actions and CI/CD workflows
│   └── workflows/
│       └── deploy.yml            # Automated deployment workflow
├── public/                       # Static assets
│   ├── favicon.ico
│   └── logo.svg
├── src/
│   ├── agents/                   # AI Agent architecture
│   │   ├── master-agent.ts       # GPT-4o based controller
│   │   ├── ethics-agent.ts       # Claude-based ethics reviewer
│   │   └── worker-agents.ts      # Specialized task agents
│   ├── ai/                       # AI model interfaces
│   │   ├── openai.ts             # OpenAI integration
│   │   ├── anthropic.ts          # Claude integration
│   │   └── mistral.ts            # Mistral fallback integration
│   ├── components/               # React components
│   │   ├── ui/                   # shadcn/ui components
│   │   │   ├── button.tsx
│   │   │   ├── card.tsx
│   │   │   └── ...
│   │   ├── layout/               # Layout components
│   │   │   ├── header.tsx
│   │   │   ├── footer.tsx
│   │   │   └── sidebar.tsx
│   │   └── ai/                   # AI-specific components
│   │       ├── agent-chat.tsx    # AI interaction interface
│   │       ├── system-monitor.tsx # AI system status
│   │       └── command-console.tsx # AI command interface
│   ├── lib/                      # Utility functions and shared code
│   │   ├── autogen/              # AutoGen integration
│   │   ├── langgraph/            # LangGraph workflows
│   │   └── utils.ts              # General utilities
│   ├── pages/                    # Next.js pages (if using pages router)
│   │   ├── api/                  # API routes
│   │   │   ├── ai/               # AI endpoints
│   │   │   └── auth/             # Auth endpoints
│   │   ├── _app.tsx
│   │   ├── index.tsx
│   │   └── dashboard.tsx
│   ├── app/                      # Next.js App Router (if using App Router)
│   │   ├── api/                  # API routes
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   └── dashboard/page.tsx
│   ├── hooks/                    # Custom React hooks
│   │   ├── use-ai.ts
│   │   └── use-agent-state.ts
│   ├── styles/                   # Global styles
│   │   └── globals.css
│   └── types/                    # TypeScript type definitions
│       └── index.ts
├── .env.example                  # Example environment variables
├── .eslintrc.json                # ESLint configuration
├── .gitignore                    # Git ignore file
├── next.config.js                # Next.js configuration
├── package.json                  # NPM package definition
├── tailwind.config.js            # Tailwind CSS configuration
├── tsconfig.json                 # TypeScript configuration
└── README.md                     # Project documentation
```