# Development Guidelines

## Tech Stack Expertise
- **Languages & Frameworks:** TypeScript, Node.js, Next.js (**App Router only**), React.
- **UI & Styling:** Shadcn UI, Radix UI, Tailwind CSS.
- Always use the **latest stable versions** of frameworks and libraries.
- Never use or suggest the **Pages Router**.

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

## Performance
- Minimize `use client`, `useEffect`, and `setState`. Favor **React Server Components (RSC)**.  
- Wrap client components in **`<Suspense>` with fallbacks**.  
- Use **dynamic imports** for non-critical components.  
- Optimize images:  
  - Always use **WebP** format.  
  - Include **width/height attributes**.  
  - Enable **lazy loading**.  
