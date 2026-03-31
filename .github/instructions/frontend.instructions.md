---
applyTo: "src/components/**,src/layouts/**,src/pages/**/*.astro,**/*.css"
---

# Frontend – instrukcje

Te instrukcje dotyczą kodu frontendowego:
- plików `.astro` oraz komponentów frameworków UI używanych jako islands (np. React/Vue/Svelte),
- stylów (CSS/Tailwind/itp.),
- warstwy prezentacji.

Zasady:
- Dla komponentów Astro:
  - Korzystaj z odseparowanego frontmatteru (`---`) i części template zgodnie z dokumentacją.
  - Używaj islands tylko tam, gdzie interakcja jest naprawdę potrzebna.
- Dla komponentów frameworków (React/Vue itp.):
  - Preferuj komponenty małe i skupione na jednym zadaniu.
  - Testuj zachowanie (Vitest + testing library) zamiast polegać na snapshotach, chyba że snapshot realnie coś chroni.
- Stylowanie:
  - Trzymaj się przyjętego systemu (np. utilitki Tailwinda / BEM / design system).
  - Nie wprowadzaj nowych patternów CSS bez uzasadnienia.
- Dostępność:
  - Używaj semantycznych tagów HTML i atrybutów ARIA tam, gdzie to potrzebne.
  - Upewnij się, że interaktywne elementy są dostępne z klawiatury i mają odpowiedni focus state.
