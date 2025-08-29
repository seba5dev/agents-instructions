# Development Guidelines

## Tech Stack Expertise
- **Languages & Frameworks:** TypeScript, Node.js, Vite, React, React Router.
- **UI & Styling:** Shadcn UI, Radix UI, Tailwind CSS.
- Always use the **latest stable versions** of frameworks and libraries.

---

## Approach
1. Start with **step-by-step pseudocode** describing the solution in detail.  
2. Confirm the plan before writing code.  
3. Deliver **accurate, factual, bug-free, fully functional, secure, and efficient** implementations.  
4. Always provide **complete solutions** (no TODOs, no placeholders).  
5. Maintain **clean, modern, and consistent code** across the project.

---

## Principles
- Prioritize **readability over raw performance**.  
- Write only the **necessary code** to achieve the requested functionality.  
- Update or create **tests** whenever functionality changes.  
- If uncertain, **state it clearly** instead of guessing.

---

## Naming Conventions
- **Directories:** use lowercase with dashes → `components/auth-wizard`.  
- **Exports:** prefer **named exports** for components.  

---

## TypeScript
- Use **TypeScript everywhere**.  
- Prefer **interfaces over types**.  
- Avoid enums → use maps or objects instead.  
- Always implement **functional components with interfaces**.  

---

## UI & Styling
- Use **Shadcn UI + Radix UI + Tailwind CSS** for components and styling.  
- Follow **mobile-first responsive design**.  

---

## Routing (React Router)
- Define routes using **React Router** with a clear folder-based structure.  
- Use **lazy loading with `React.lazy`** and `Suspense` for code splitting.  
- Implement **loaders and actions** where appropriate for data fetching and mutations.  
- Keep routes **modular and minimal** (avoid deeply nested complexity unless required).  

---

## Performance
- Use **Vite plugins** (e.g., `@vitejs/plugin-react`) to optimize builds.  
- Leverage **React Router’s lazy + Suspense** for route-based code splitting.  
- Minimize unnecessary `useEffect` and `setState`. Favor derived state and memoization.  
- Optimize images:  
  - Always use **WebP** format.  
  - Include **width/height attributes**.  
  - Enable **lazy loading**.  
- Enable **Vite aliasing** for cleaner imports (e.g., `@/components/...`).  

---

## Extra (Vite-specific)
- Use `.env` files with **`import.meta.env`** for environment variables.  
- Configure `vite.config.ts` for **path aliases**, **plugins**, and **build optimization**.  
- Use **`vite preview`** before deployment to test production build locally.  
