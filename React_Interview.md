# React / Frontend Interview Master Guide

> Consolidated from all interview question sets shared in this chat.
>
> **Target profile:** 4+ years Frontend / React experience, answering at senior-level depth without overstating experience.
>
> **How to use this guide:** For each topic, learn the **2-minute answer** first, then the deeper explanation, code, trade-offs, and follow-ups. For behavioral questions, replace generic wording with your real project incident whenever possible.

---

## Table of Contents

1. Question Inventory — every question/topic shared
2. Professional Introduction & Project Experience
3. Core JavaScript
4. TypeScript
5. React Fundamentals & Internals
6. React Hooks, State & Component Design
7. Redux, Context, TanStack Query & Data Strategy
8. Next.js / Rendering / Hydration
9. Browser Rendering, CSS & Performance
10. Build Tools, Bundle Optimization & Web Vitals
11. Accessibility / WCAG
12. Testing
13. Web Security / Authentication / RBAC
14. API Strategy, Caching, Retries, Rate Limits & BFF
15. Angular / RxJS / Node.js / Express Topics
16. CI/CD / GitHub Actions
17. SEO
18. Frontend Architecture & Scalability
19. Frontend System Design
20. Coding Appendix
21. Managerial / Behavioral / STAR Answers
22. Final Senior-Level Interview Framework

---

# 1. Question Inventory — Every Question/Topic Shared

This section preserves the question themes from every list you shared. Near-duplicates are consolidated into one canonical answer later in the guide.

## Senior Frontend / Architect Topics

- Architecture & Scalability
- Performance Optimization
- State Management Strategy
- Component System Design
- Routing & Rendering Strategy
- Cross-platform Compatibility
- Debugging Production Issues
- Frontend Security
- API & Data Strategy
- Testing Strategy

## React Internals Topics

- Hydration errors in Next.js
- Why server HTML mismatches client render
- Why components re-render even if props don't change
- What happens internally when `setState` is called
- Diffing and React reconciliation
- Stale closures
- How to debug React performance
- When NOT to use `useMemo` / `useCallback`
- Server Components
- Keys in React lists
- How to scale a component/application for 1M users

## Accessibility Topics

- Semantic HTML
- Keyboard accessibility
- Screen-reader accessibility
- Focus management
- Color contrast
- Responsive readability
- Reduced motion
- Accessible forms
- Live regions
- Accessibility testing

## Resume / Project-Based Questions

- How did you optimize Redux Toolkit + Redux Saga performance?
- Next.js SSR vs SSG for sports betting odds
- Authentication and role-based access
- How did you debug excessive React re-renders?
- How did you use Google Tag Manager and measure performance?

## JavaScript / React / Architecture Question Set

- Explain closures
- Explain hoisting
- Callback hell
- Redux architecture
- Promise vs async/await
- React performance
- `forwardRef`
- Compound Components
- `children` props
- Middleware
- API handling
- JWT flow
- Virtual DOM
- React keys
- React Portals
- Explain your current project architecture
- Find the first unique character

## Deloitte-Style Questions

- Arrow functions
- Event loop
- Callback queues
- Hoisting
- Generator functions
- Closures
- JavaScript output questions
- Flatten nested arrays
- `map` / `filter` / `reduce` / `forEach`
- Why React re-renders
- How to prevent unnecessary renders
- `useEffect` vs `useLayoutEffect`
- Controlled vs uncontrolled components
- React performance optimization
- Authentication flow
- Redux Toolkit

## Licious Managerial / Technical Questions

- SSE vs WebSockets
- Bundle-size analysis and optimization
- gRPC vs JSON
- Conflict with backend team
- Walk through previous projects
- SSR and SEO
- Performance optimizations implemented
- Tree-shaking algorithm / internals
- BFF architecture

## Persistent Systems Question Set

- Event loop and asynchronous execution
- Custom debounce hook
- Reusable searchable multi-select dropdown
- React rendering performance for 10k+ rows
- Controlled vs uncontrolled components
- Scalable React application with 100+ pages
- Code splitting and lazy loading
- Frontend API rate-limit handling
- Hydration and UI mismatches
- Component library for multiple teams
- CSR vs SSR vs SSG
- Frontend architecture for 1M+ daily users
- Critical production bug
- Technical debt vs features
- Conflict with designers/backend
- Communicating technical decisions to non-technical stakeholders

## Additional Frontend Platform Topics

- Browser rendering pipeline
- Vite
- Webpack
- WCAG
- Testing
- GitHub Actions
- CI/CD
- XSS
- Web Vitals
- SEO

## L1 Question Set

- Introduce yourself
- Implement `chunk<T>(items, size)`
- Deep vs shallow copy
- What are primitives?
- Spread vs rest
- What is a Promise?
- Union types
- Types of interfaces
- Dependency Injection in Angular
- Standalone Components vs NgModules
- `switchMap` vs `mergeMap`
- Async Pipe
- `process.nextTick()`
- Event Loop
- Buffers
- Secure Express route
- Unit-testing plan for a new feature
- What have you done with Copilot?

## Technical Rounds Question Set

- JavaScript execution context, call stack and event loop
- Closures, hoisting, Promises, async/await
- Arrow vs normal functions
- Array/string methods
- Top-K elements
- HashMap DSA problem
- Expand/collapse React list
- Reusable Button with variants/sizes
- Class lifecycle and Hooks
- Reconciliation and rendering
- Event bubbling vs capturing
- Reflow vs repaint
- Why transform is preferred for CSS animations
- How browser renders a webpage
- Large lists / thousands of items
- Virtualization / windowing
- Frontend performance techniques
- Promise polyfill
- Async scheduler with maximum concurrency
- Internal asynchronous execution
- React-like class component using ES5

## Frontend HLD Question Set

- Pinterest-like grid UI
- Component breakdown and architecture
- Data flow between components
- Large dataset handling
- Pagination / infinite scrolling
- Caching and API integration
- Performance optimization
- Component hierarchy and reusability
- HLD of an existing/past project
- API contracts
- State management
- Caching and error handling
- Non-functional requirements: performance, scalability, availability, response time

## System Design Question Set

- Real-time collaborative text editor like Google Docs
- Rate limiter for API calls in a SPA
- Dynamic pagination / infinite scrolling
- Client-side state management system like Redux Toolkit
- Social login + OAuth + JWT authentication flow
- Scalable notification system

---

# 2. Professional Introduction & Project Experience

## Q1. Introduce yourself / Tell me about yourself.

### Interview-ready answer

> "I'm a frontend developer with 4+ years of experience, primarily focused on React.js, JavaScript, state management, responsive UI development, API integration and frontend performance.
>
> I've worked on applications involving reusable component development, Redux and Redux Toolkit, Redux-Saga for asynchronous workflows, routing, authentication, analytics integration and performance optimization. I've also worked with tools and technologies such as Tailwind CSS, Material UI, REST APIs, Firebase, Google Tag Manager and Meta Pixel.
>
> Some of my project work has included data-driven dashboards, a voice-based interview application, and consumer-facing React applications with features such as cart state, infinite scrolling and API integration.
>
> My strongest area is React and JavaScript, especially component architecture, state management, asynchronous flows and debugging frontend performance issues. I'm also strengthening my knowledge of Next.js, Node.js and system design so that I can reason about the complete frontend-to-backend architecture rather than only the UI layer."

### Follow-up: "What is your strongest area?"

> "React and JavaScript are my strongest areas, particularly component architecture, state management, API integration and performance optimization."

---

## Q2. Why React.js?

### Answer

React is primarily a UI library built around component-based development and declarative rendering.

I would choose React because it provides:

- Component-based architecture
- Declarative UI
- A strong ecosystem
- Good support for reusable design systems
- Flexible state-management choices
- Strong developer tooling
- Good integration with routing, data-fetching and full-stack frameworks

### Senior-level answer

> "I like React because it gives a strong component model without forcing the whole application architecture into one rigid pattern. That flexibility is useful for large applications because we can choose appropriate solutions for local state, global client state and server state separately."

---

## Q3. What roles and responsibilities did you have in your projects?

Use a responsibility-based answer rather than a list of technologies.

> "My responsibilities have included breaking requirements into frontend components, implementing reusable and responsive UI, integrating REST APIs, handling client and server-related state, implementing authentication flows, working with Redux / Redux Toolkit / Redux-Saga, debugging production issues, optimizing rendering and network performance, integrating analytics such as GTM and Meta Pixel, and collaborating with backend, QA and product/design teams.
>
> I also participate in code reviews and try to improve maintainability through reusable components, consistent patterns and clear separation between UI logic, state logic and API communication."

Do not claim ownership of architecture, code reviews, releases or team leadership unless you actually did those things.

---

## Q4. Walk through your previous projects.

Use this order:

```text
Business problem
↓
Users
↓
Key features
↓
Frontend architecture
↓
State management
↓
API layer
↓
Authentication
↓
Performance
↓
Challenges
↓
Your contribution
↓
What you learned / would improve
```

### Example: Food / Swiggy-style React application

> "I worked on a React SPA where the goal was to provide a food-discovery and ordering experience. The UI consumed restaurant data from an API, and I handled component rendering, routing, cart state, shimmer/loading states and infinite scrolling. Redux was used for cart-related state, while Tailwind was used for styling and Parcel for bundling. A key consideration was keeping the UI responsive while handling dynamic lists and asynchronous API responses."

### Example: Voice-Based Interview Application

> "Another project was a voice-based interview application using React along with Dialogflow, Firebase and speech-to-text/text-to-speech capabilities. The frontend had to coordinate asynchronous interactions, user input, feedback and analytics. This project helped me think more carefully about state transitions, async error handling and user experience during long-running operations."

### Example: EV dashboard / API work

> "I also worked on an EV dashboard-related React task involving API integration, retries and fetching data from a backend endpoint. The main focus there was reliable async behavior and predictable UI handling when network calls did not succeed on the first attempt."

---

# 3. Core JavaScript

## Q5. What are primitives in JavaScript?

There are seven primitive types:

```text
string
number
bigint
boolean
undefined
symbol
null
```

Primitives are immutable values. Objects, arrays and functions are non-primitive reference values.

```js
const a = 10;
const b = a;
```

Changing `b` does not change `a`.

### Senior point

`number` includes integers and floating-point values; `bigint` is used for arbitrarily large integers; `symbol` provides unique primitive identifiers.

---

## Q6. `let` vs `const` vs `var`; hoisting and Temporal Dead Zone

| Keyword | Scope | Reassignment | TDZ | Function/global behavior |
|---|---|---:|---:|---|
| `var` | Function | Yes | No | Function-scoped; older semantics |
| `let` | Block | Yes | Yes | Block-scoped |
| `const` | Block | No | Yes | Block-scoped |

```js
console.log(a); // undefined
var a = 10;
```

But:

```js
console.log(b); // ReferenceError
let b = 10;
```

The declaration exists in the lexical environment, but access before initialization occurs inside the Temporal Dead Zone.

### Important nuance

Hoisting does not mean the source code is literally moved to the top. It refers to how declarations are created and made available as execution context setup occurs.

---

## Q7. Explain closures. Give a real-world use case.

A closure is a function together with access to variables in its lexical environment.

```js
function createCounter() {
  let count = 0;

  return function increment() {
    count += 1;
    return count;
  };
}

const counter = createCounter();

console.log(counter()); // 1
console.log(counter()); // 2
```

The returned function retains access to `count`.

### Real-world uses

- Private state
- Event handlers
- Debouncing / throttling
- Memoization
- Factories
- React callbacks and effects

### Stale closure vs memory leak

A **stale closure** means a callback retained an older lexical value and therefore behaves with outdated state.

A **memory leak** means objects remain reachable and consume memory even though the application no longer needs them.

They are related through reachability, but not the same problem.

---

## Q8. Why can a long chain of resolved Promises still freeze the UI?

Promise continuations run as microtasks. The browser drains microtasks before continuing to the next task/render opportunity. If JavaScript continuously creates microtasks or performs heavy CPU work, the main thread can remain busy and rendering can be delayed.

```js
function loop() {
  Promise.resolve().then(loop);
}

loop();
```

This can starve the browser because control keeps returning to the microtask queue.

### Senior answer

> "Asynchronous does not mean non-blocking. Promise callbacks don't magically run on another CPU thread. They still execute JavaScript on the main thread, so a sufficiently large microtask workload can delay input handling and rendering."

### Better solutions for CPU-heavy work

- Split work into chunks
- Use `setTimeout` / `scheduler`-style yielding where suitable
- Use `requestAnimationFrame` for frame-related work
- Use Web Workers for CPU-heavy tasks that can be moved off the main thread

---

## Q9. Explain the JavaScript Event Loop.

A good browser-level model is:

```text
Call Stack
   ↓
Host / Web APIs
   ↓
Callbacks become ready
   ↓
Microtask Queue   ← Promise.then / queueMicrotask
   ↓
Task Queue        ← timers / events and other tasks
   ↓
Rendering opportunity
```

Exact scheduling details differ between browsers and Node.js, so avoid claiming there are only two universal queues.

Example:

```js
console.log("A");

setTimeout(() => console.log("B"), 0);

Promise.resolve().then(() => console.log("C"));

console.log("D");
```

Output:

```text
A
D
C
B
```

---

## Q10. Explain Microtasks vs Macrotasks / Tasks.

### Microtasks

Examples:

```text
Promise.then
Promise.catch
Promise.finally
queueMicrotask
```

### Tasks / macrotasks

Examples include:

```text
setTimeout callbacks
user events
some I/O-related callbacks depending on host
```

### Interview answer

> "After the current JavaScript stack completes, microtasks are given high priority and are generally drained before the next task is taken. That's why Promise continuations commonly execute before a `setTimeout(..., 0)` callback."

---

## Q11. What is `===` vs `==`? Explain type coercion.

`===` checks strict equality without implicit type coercion.

`==` performs the Abstract Equality Comparison, which can coerce types.

```js
0 == false;   // true
0 === false;  // false

"1" == 1;    // true
"1" === 1;   // false

null == undefined;  // true
null === undefined; // false
```

### Best practice

Prefer `===` unless you intentionally want the semantics of `==` and fully understand the coercion rule involved.

---

## Q12. Arrow functions vs normal functions

### Main differences

- Arrow functions have lexical `this`
- Arrow functions do not have their own `arguments`
- Arrow functions cannot be used as constructors
- Arrow functions don't have a `prototype` used for construction
- Normal functions derive `this` from invocation context

```js
const obj = {
  name: "Shubham",
  normal() {
    console.log(this.name);
  },
  arrow: () => {
    console.log(this.name);
  }
};
```

The arrow's `this` comes from the outer lexical context, not from `obj`.

---

## Q13. What is a Promise?

A Promise represents an eventual result of an asynchronous operation.

States:

```text
pending
  ↓
fulfilled

or

rejected
```

```js
const promise = fetch("/api/users");

promise
  .then(res => res.json())
  .then(data => console.log(data))
  .catch(error => console.error(error));
```

### Important

An `async` function always returns a Promise, even when it returns a plain value.

---

## Q14. Promises vs async/await

`async/await` is syntax built around Promise-based asynchronous control flow.

```js
async function getUsers() {
  try {
    const response = await fetch("/api/users");
    return await response.json();
  } catch (error) {
    console.error(error);
    throw error;
  }
}
```

Promises:

```js
fetch(url)
  .then(...)
  .catch(...);
```

Async/await is often easier to read for sequential async workflows.

### Event-loop point

The continuation after `await` is scheduled through Promise machinery and therefore resumes asynchronously; it is not a synchronous blocking wait.

---

## Q15. Why does an error inside an asynchronous callback escape the surrounding try/catch?

This does not work:

```js
try {
  setTimeout(() => {
    throw new Error("Boom");
  }, 0);
} catch (error) {
  console.log("Caught");
}
```

The `try` block has already completed before the timer callback executes.

Correct handling:

```js
setTimeout(() => {
  try {
    throw new Error("Boom");
  } catch (error) {
    console.error(error);
  }
}, 0);
```

Or with Promises:

```js
fetch(url)
  .then(...)
  .catch(error => {
    console.error(error);
  });
```

Or with `await`:

```js
try {
  const response = await fetch(url);
} catch (error) {
  console.error(error);
}
```

### Senior answer

> "A try/catch only catches errors thrown during the synchronous execution of its protected block, unless the asynchronous operation is awaited or the callback establishes its own error-handling path."

---

## Q16. Explain spread vs rest operators.

The syntax is the same (`...`) but the role is different.

### Spread — expands

```js
const a = [1, 2];
const b = [...a, 3];
```

### Rest — collects

```js
function sum(...numbers) {
  return numbers.reduce((total, n) => total + n, 0);
}
```

Interview shortcut:

> **Spread expands; rest collects.**

### Important

Object/array spread performs shallow copying. It does not recursively deep-clone nested references.

---

## Q17. Deep copy vs shallow copy. Where can the shared reference remain?

```js
const user = {
  name: "A",
  address: {
    city: "Delhi"
  }
};

const copy = { ...user };
```

Top-level object is new, but:

```js
user.address === copy.address // true
```

Therefore:

```js
copy.address.city = "Mumbai";
```

also changes the nested object visible through `user`.

### Deep copy

```js
const copy = structuredClone(user);
```

`JSON.parse(JSON.stringify(...))` is not a general-purpose deep clone because it loses or mishandles values such as `undefined`, functions, `Date`, `Map`, `Set`, and other non-JSON data.

---

## Q18. `nullish coalescing (??)` vs logical OR (`||`).

`||` falls back when the left side is **falsy**.

`??` falls back only when the left side is **null or undefined**.

```js
const a = 0 || 10;   // 10
const b = 0 ?? 10;   // 0

const c = "" || "default"; // "default"
const d = "" ?? "default"; // ""
```

Use `??` when values such as `0`, `false` and `""` are legitimate values and should not be replaced.

---

## Q19. WeakMap and WeakSet

### WeakMap

A WeakMap stores key/value pairs where the keys must be objects or non-registered symbols, and the collection does not prevent eligible object keys from being garbage-collected.

Typical use cases:

- Metadata associated with object instances
- Private-ish library state keyed by objects
- Caches where entries should disappear when the key becomes unreachable

```js
const metadata = new WeakMap();

const element = {};
metadata.set(element, { mountedAt: Date.now() });
```

### WeakSet

Stores weakly held object-like members, useful for tracking object identity such as:

```js
const visited = new WeakSet();
```

### Important limitation

Weak collections are not iterable and don't expose normal collection enumeration because garbage collection can make membership disappear nondeterministically.

---

## Q20. Event delegation — how does it work and why is it efficient?

Event delegation takes advantage of event bubbling: instead of attaching a listener to every child, attach a listener to a common ancestor and inspect the target.

```html
<ul id="list">
  <li data-id="1">One</li>
  <li data-id="2">Two</li>
</ul>
```

```js
list.addEventListener("click", event => {
  const item = event.target.closest("li[data-id]");

  if (!item) return;

  console.log(item.dataset.id);
});
```

### Why efficient?

If there are thousands of children, you can often avoid thousands of individual listeners. One ancestor listener handles events for many descendants.

### Senior nuance

Delegation is not automatically better for every case. The event must bubble or be handled appropriately, and selectors/target traversal should remain cheap.

---

## Q21. Event bubbling vs capturing

Propagation has three conceptual phases:

```text
Capture
window → document → parent → target

Target

Bubble
parent ← document ← window
```

Capture listener:

```js
parent.addEventListener("click", handler, {
  capture: true
});
```

Bubble listener:

```js
parent.addEventListener("click", handler);
```

In React, event handling is designed around a delegation-style synthetic event system, although implementation details have evolved across React versions.

---

## Q22. How do you handle multiple simultaneous messages in a real-time chat without blocking the main thread?

Use a pipeline:

```text
WebSocket/SSE
   ↓
Buffer / queue
   ↓
Batch incoming messages
   ↓
Update state once per frame/batch
   ↓
Virtualized list
```

### Practical strategy

1. Buffer bursts of messages.
2. Batch state updates.
3. Virtualize the message list when it becomes large.
4. Avoid expensive sorting/filtering during every message arrival.
5. Keep message state normalized where appropriate.
6. Move CPU-heavy parsing/transformation to a Web Worker if necessary.
7. Use `requestAnimationFrame` or another yielding strategy for frame-sensitive work.

The goal is to avoid doing:

```text
1 message
→ render
→ layout
→ paint
→ 2nd message
→ render
→ layout
→ paint
```

when a burst can be consolidated.

---

# 4. TypeScript

## Q23. What are union types?

A union allows a value to be one of several types.

```ts
let id: string | number;

id = "123";
id = 123;
```

String-literal unions are particularly useful for finite states:

```ts
type Status = "loading" | "success" | "error";
```

### Senior use

Union types are useful for modeling state machines and API states, and can be narrowed using `typeof`, `in`, discriminants or user-defined type guards.

---

## Q24. What are different types of interfaces?

TypeScript doesn't formally categorize interfaces into a fixed list called "types of interfaces." A better answer is to describe common interface forms.

### Object shape

```ts
interface User {
  id: number;
  name: string;
}
```

### Optional / readonly

```ts
interface User {
  readonly id: number;
  name?: string;
}
```

### Function signature

```ts
interface Calculator {
  (a: number, b: number): number;
}
```

### Extension

```ts
interface Employee extends User {
  department: string;
}
```

### Multiple extension

```ts
interface Employee extends User, Auditable {
  department: string;
}
```

### Interface vs type alias

Both can model object shapes. Interfaces support declaration merging and are often natural for object contracts; type aliases are especially flexible for unions, intersections, tuples and conditional/mapped compositions.

---

## Q25. TypeScript Generics

Generics let a function/type preserve relationships between input and output types.

```ts
function identity<T>(value: T): T {
  return value;
}

const n = identity(10);      // number
const s = identity("hello"); // string
```

### Constraint

```ts
function getLength<T extends { length: number }>(value: T) {
  return value.length;
}
```

Generics are useful for reusable API clients, hooks, utility functions, data tables and component libraries.

---

## Q26. Utility types: Partial, Pick, Omit, Record

### Partial

Makes properties optional.

```ts
type UserUpdate = Partial<User>;
```

### Pick

Selects properties.

```ts
type UserSummary = Pick<User, "id" | "name">;
```

### Omit

Removes properties.

```ts
type PublicUser = Omit<User, "password">;
```

### Record

Maps keys to a common value type.

```ts
type StatusMessage = Record<"loading" | "error", string>;
```

---

# 5. React Fundamentals & Internals

## Q27. What is the Virtual DOM?

The Virtual DOM is a useful conceptual description of React's in-memory representation of UI elements. React compares the new element tree with the previous one and determines the necessary host-environment updates.

It is **not** simply "a faster DOM." The real benefit comes from declarative programming, component composition and React's ability to schedule/reconcile updates efficiently.

---

## Q28. Explain React Reconciliation / diffing.

When React receives a state/prop/context update, it calculates the next element tree and reconciles it against the previous tree.

A simplified mental model:

```text
State/props update
      ↓
Render phase
      ↓
New element tree
      ↓
Reconciliation
      ↓
Commit phase
      ↓
Host DOM updates
```

Important heuristics include:

- Element type changes can cause a subtree to be replaced.
- Stable `key` values provide list-item identity.
- React uses its own reconciliation rules rather than comparing every possible DOM node pair with a mathematically optimal diff.

---

## Q29. What is React Fiber?

Fiber is React's internal architecture for representing work in a way that supports scheduling and prioritization.

Conceptually it allows React to:

- Break rendering work into units
- Track work and priority
- Pause/yield render work in concurrent scenarios
- Resume or abandon work before committing
- Coordinate updates with modern React features

### Important distinction

Fiber is not a second DOM.

It is an internal data structure/architecture used to represent React's work and component tree.

---

## Q30. What is Concurrent Rendering?

Concurrent rendering means React can work on rendering in an interruptible way rather than treating every render as one indivisible synchronous block.

This allows urgent user interactions to be prioritized over less urgent work.

It does **not** mean two JavaScript functions execute simultaneously on the same main thread.

### Example concept

```text
Urgent input
   ↓
Prioritize
   ↓
Render lightweight update

Background transition
   ↓
Can be interrupted/restarted
```

---

## Q31. What are the latest React features and updates?

**Current note for this handbook: the React documentation lists React 19.3 as the latest version.** React's official September 2026 release notes highlight features including **View Transitions, Fragment Refs, `browser()`, Trusted Types support and additional Server Components improvements**. React 19 introduced Actions, `useActionState`, `useOptimistic`, form Actions and `ref` as a prop for function components. citeturn264643search6turn264643search3turn264643search0

### Features you should know

#### Actions / async actions

React 19 introduced a model for handling async mutations with pending state, optimistic updates and errors.

#### `useActionState`

Helps manage an action's result and pending state.

#### `useOptimistic`

Provides a supported pattern for optimistic UI while an async action is pending.

#### Form Actions

React 19 added Action integration to form submission APIs.

#### `ref` as a prop

Function components can receive `ref` as a prop in React 19, reducing the need for `forwardRef` in new code. React's documentation notes that `forwardRef` is planned for future deprecation/removal as this model evolves. citeturn264643search0

#### Server Components

React Server Components allow components to render in a server environment separate from the client application, when the framework/bundler supports them. citeturn264643search0

#### React 19.3 additions

Know the headline additions such as View Transitions, Fragment Refs, `browser()` and Trusted Types, but explain only the ones relevant to the role. citeturn264643search3

### Interview answer

> "I keep up with React through the official release notes. Today I'd be comfortable discussing React 19 features such as Actions, `useActionState`, `useOptimistic`, form Actions, Server Components, and the current React 19.3 additions such as View Transitions and Fragment Refs. I also distinguish framework-specific features such as Next.js Server Components from core React APIs."

---

## Q32. What happens internally when `setState` is called?

For function components, think of `setState` as scheduling a state update rather than immediately mutating the local variable from the current render.

Conceptually:

```text
setState(update)
      ↓
Update queued
      ↓
React schedules work
      ↓
Render phase
      ↓
Compute next tree
      ↓
Commit phase
      ↓
DOM updated
      ↓
Effects run at appropriate time
```

This is why:

```js
setCount(count + 1);
console.log(count);
```

does not imply the local `count` variable immediately changes in the current render.

### Functional updater

```js
setCount(prev => prev + 1);
```

is important when the new state depends on the previous queued state.

---

## Q33. Why use `setCount(prev => prev + 1)` instead of `setCount(count + 1)`?

Consider:

```js
setCount(count + 1);
setCount(count + 1);
```

Both expressions can calculate the same next value from the same render snapshot.

Instead:

```js
setCount(prev => prev + 1);
setCount(prev => prev + 1);
```

lets React apply the updates sequentially to the pending state.

Conceptually:

```text
initial = 0

update 1: prev → 1
update 2: prev → 2
```

### Interview answer

> "When the next state depends on the previous state, I prefer the functional updater because it composes correctly with queued/batched updates and avoids relying on a potentially stale render snapshot."

---

## Q34. Why do components re-render even if props don't change?

A component can re-render because:

- Its own state changed
- Its parent rendered and the child was rendered again
- Context value changed
- A subscribed store/query changed
- A hook caused an update
- A new element/function/object identity changes downstream behavior

`React.memo` can skip a child when its props are considered equal, but it does not prevent updates caused by the child's own state or context usage.

### Important

"Props didn't change" does not mean "the component has no reason to render."

---

## Q35. How do you prevent unnecessary re-renders?

Start with measurement.

Tools:

- React DevTools Profiler
- Chrome Performance panel
- Render highlighting / component tracing where useful

Techniques:

- Keep state as local as practical
- Split large components
- Avoid unnecessary Context provider churn
- Use `React.memo` when prop stability makes it effective
- Use `useMemo` / `useCallback` only where they reduce meaningful downstream work
- Use memoized selectors for derived state
- Normalize large state where appropriate
- Virtualize large lists

### Senior answer

> "I don't start by memoizing everything. I identify which component or calculation is expensive and why it is re-rendering, then apply the smallest technique that addresses the measured bottleneck."

---

## Q36. When should you NOT use `useMemo` or `useCallback`?

Do not use them automatically.

Bad example:

```js
const total = useMemo(() => a + b, [a, b]);
```

if the calculation is trivial and there is no meaningful downstream benefit.

Memoization itself has costs:

- Dependency comparison
- Memory retention
- More code complexity
- More cognitive overhead

`useCallback` is especially useful when a function's identity matters to a memoized child or another hook dependency.

### Interview answer

> "I use memoization when it prevents expensive work or stabilizes an identity that matters. If the calculation is cheap or dependencies change frequently, memoization can make the code slower or more complex without producing a measurable win."

---

## Q37. `useRef` vs `useState`

### `useState`

- State changes trigger re-rendering.
- Used for data that affects rendered UI.

### `useRef`

- Holds a mutable `.current` value.
- Updating `.current` does not trigger a render.
- Useful for DOM references and mutable values that should persist across renders without driving the UI.

```jsx
const countRef = useRef(0);
countRef.current += 1;
```

versus:

```jsx
const [count, setCount] = useState(0);
setCount(prev => prev + 1);
```

### Rule

If changing the value should cause the UI to update, use state. If it is imperative/mutable data that does not define the rendered output, a ref may be appropriate.

---

## Q38. `useEffect` vs `useLayoutEffect`

### `useEffect`

Runs after the commit and generally after the browser has had an opportunity to paint.

Use it for:

- data fetching
- subscriptions
- logging
- synchronization with external systems

### `useLayoutEffect`

Runs after DOM mutations but before the browser paints the updated screen.

Use it when you must measure or synchronously adjust layout before the user sees the frame.

Example:

```jsx
useLayoutEffect(() => {
  const rect = ref.current.getBoundingClientRect();
  setPosition(rect.height);
}, []);
```

### Caution

Overusing `useLayoutEffect` can block painting. In server rendering contexts, browser-only layout effects also require careful handling because there is no layout environment on the server.

---

## Q39. How does React handle effect dependency cycles / circular dependencies?

Usually the problem is not React detecting a mathematical cycle; it's the effect updating state that changes one of its own dependencies.

Example:

```jsx
useEffect(() => {
  setValue(value + 1);
}, [value]);
```

This creates:

```text
render
 ↓
effect
 ↓
setValue
 ↓
render
 ↓
effect
 ↓
...
```

### How to prevent it

- Remove unnecessary effects
- Derive values during rendering instead of storing derived state
- Use correct dependencies
- Use functional updates where appropriate
- Separate synchronization effects from calculations

The deeper principle is: **effects should synchronize React with external systems, not be used as a default mechanism for deriving internal state.**

---

## Q40. What are React keys and why are they important?

Keys give list items stable identity across renders.

```jsx
items.map(item => (
  <Row key={item.id} item={item} />
));
```

Using array indices as keys can be problematic when a list is reordered, inserted into or filtered because identity follows the position rather than the logical item.

### Interview answer

> "Keys are not primarily about silencing a warning; they tell React which logical item is which across renders, which affects state preservation and reconciliation behavior."

---

## Q41. What happens if the element type changes during reconciliation?

For example:

```jsx
<div>...</div>
```

becomes:

```jsx
<section>...</section>
```

React's reconciliation rules treat a different element type as a structural change, which can cause the corresponding subtree to be replaced rather than updated in place.

That's why stable component/element structure matters when preserving local state.

---

## Q42. Explain React Portals.

A portal renders React content into a DOM node outside the normal DOM position of the component while preserving React's logical relationship.

```jsx
createPortal(
  <Modal />,
  document.getElementById("modal-root")
);
```

Common use cases:

- Modals
- Tooltips
- Toasts
- Popovers

Useful because CSS stacking/overflow constraints can make rendering inside the normal DOM subtree awkward.

---

## Q43. `forwardRef` and the current React model

Historically:

```jsx
const Input = forwardRef((props, ref) => (
  <input ref={ref} />
));
```

React 19 allows a function component to receive `ref` as a prop directly:

```jsx
function Input({ ref, ...props }) {
  return <input ref={ref} {...props} />;
}
```

The official React 19 release notes describe `ref` as a prop for function components and note a future deprecation/removal direction for `forwardRef` in new code. citeturn264643search0

---

## Q44. Compound Components

Compound components allow a component family to share behavior/state through composition.

Example API:

```jsx
<Tabs>
  <Tabs.List>
    <Tabs.Trigger value="one">One</Tabs.Trigger>
    <Tabs.Trigger value="two">Two</Tabs.Trigger>
  </Tabs.List>

  <Tabs.Content value="one">...</Tabs.Content>
</Tabs>
```

Internally, Context can coordinate shared state.

### Benefits

- Flexible composition
- Good developer experience
- Encapsulated coordination
- Reusable component primitives

### Trade-off

Too much implicit behavior can make debugging harder, so document the component contract carefully.

---

## Q45. `children` prop

`children` is a normal React prop used for composition.

```jsx
<Card>
  <h2>Hello</h2>
</Card>
```

Inside:

```jsx
function Card({ children }) {
  return <section>{children}</section>;
}
```

It enables composition without forcing a component to know the exact contents of its children.

---

## Q46. Custom Hooks

A custom hook extracts reusable stateful logic.

Example:

```jsx
function useOnlineStatus() {
  const [online, setOnline] = useState(navigator.onLine);

  useEffect(() => {
    const onOnline = () => setOnline(true);
    const onOffline = () => setOnline(false);

    window.addEventListener("online", onOnline);
    window.addEventListener("offline", onOffline);

    return () => {
      window.removeEventListener("online", onOnline);
      window.removeEventListener("offline", onOffline);
    };
  }, []);

  return online;
}
```

### Principle

Custom hooks share **logic**, not component instance state.

---

## Q47. Custom debounced-value hook

```jsx
import { useEffect, useState } from "react";

function useDebounce(value, delay = 300) {
  const [debouncedValue, setDebouncedValue] = useState(value);

  useEffect(() => {
    const timer = setTimeout(() => {
      setDebouncedValue(value);
    }, delay);

    return () => clearTimeout(timer);
  }, [value, delay]);

  return debouncedValue;
}
```

Usage:

```jsx
function Search() {
  const [query, setQuery] = useState("");
  const debouncedQuery = useDebounce(query, 300);

  useEffect(() => {
    if (!debouncedQuery) return;
    searchApi(debouncedQuery);
  }, [debouncedQuery]);

  return (
    <input
      value={query}
      onChange={e => setQuery(e.target.value)}
    />
  );
}
```

---

# 6. React State Management / Data Strategy

## Q48. `useState` vs `useReducer`

### `useState`

Best for simple local state:

```js
const [open, setOpen] = useState(false);
```

### `useReducer`

Useful when state has several related transitions or when actions describe domain events.

```js
const [state, dispatch] = useReducer(reducer, initialState);
```

Example actions:

```text
ADD_ITEM
REMOVE_ITEM
UPDATE_QUANTITY
CLEAR_CART
```

### Interview answer

> "If the component has a small amount of independent state, I use `useState`. If there are many related transitions, state invariants or action-driven updates, `useReducer` can make the state machine clearer."

---

## Q49. Redux architecture

A classic Redux flow is:

```text
UI
 ↓
dispatch(action)
 ↓
middleware
 ↓
reducer
 ↓
store
 ↓
selector
 ↓
UI
```

Redux enforces predictable one-way state transitions.

### Redux Toolkit

RTK simplifies Redux with:

- `configureStore`
- `createSlice`
- `createAsyncThunk`
- `createEntityAdapter`
- RTK Query

---

## Q50. Redux middleware

Middleware sits between dispatch and the reducer.

```text
dispatch(action)
      ↓
middleware
      ↓
reducer
```

Use cases:

- Async workflows
- Logging
- Analytics
- Error reporting
- Side effects

Example concept:

```js
const logger = store => next => action => {
  console.log("dispatching", action);
  return next(action);
};
```

---

## Q51. Redux Toolkit vs Context API vs TanStack Query

The correct answer is not "which is best?" They solve different problems.

| Tool | Best suited for |
|---|---|
| Context | Dependency/configuration and relatively low-frequency shared client state |
| Redux Toolkit | Complex client-side state, predictable events, cross-feature state, rich middleware needs |
| TanStack Query | Server state: fetching, caching, refetching, stale data, mutations |

### Example split

```text
Auth/session metadata → Context or Redux
UI preferences        → Context / local state
Shopping cart         → Redux/local state depending on requirements
Products/users API    → TanStack Query
```

Do not put all server data in Redux merely because Redux is already installed.

---

## Q52. Redux + Redux-Saga performance optimization

For a large application:

### Normalize data

```text
entities
  usersById
  productsById
ids
```

RTK's `createEntityAdapter` can help normalize collections.

### Memoized selectors

Use Reselect-style selectors to avoid recomputing expensive derived data.

### Narrow subscriptions

Avoid subscribing a huge component tree to one frequently changing slice.

### Saga optimization

Use operators according to semantics:

```text
takeLatest  → latest request matters
 takeEvery  → every event matters
     call   → invoke async function
      put   → dispatch action
```

### Interview answer

> "I optimize Redux first by reducing the number and size of updates reaching unrelated components, then by memoizing expensive derived data and choosing saga concurrency operators according to the business behavior. I profile before adding memoization."

---

## Q53. `switchMap` vs `mergeMap`

### `switchMap`

New inner observable cancels/unsubscribes the previous inner subscription.

Great for search:

```text
r    → request A
re   → cancel A, request B
rea  → cancel B, request C
```

### `mergeMap`

Allows multiple inner observables to run concurrently.

Good when every operation matters and can overlap.

### Related operators

```text
switchMap  → latest
mergeMap   → concurrent
concatMap  → sequential queue
exhaustMap → ignore new while current runs
```

---

## Q54. Optimistic vs pessimistic updates

### Optimistic

Update UI immediately, send server request, rollback on failure.

```text
User action
   ↓
Optimistic UI
   ↓
API mutation
   ├── success → keep
   └── failure → rollback
```

Good for low-latency-feeling interactions such as likes, toggles and cart updates where rollback is well-defined.

### Pessimistic

Wait for server success before reflecting the final state.

Useful when correctness must reflect server confirmation before changing the UI.

---

## Q55. API caching, retries and background sync

A mature data layer can handle:

- Query-key-based caching
- Deduplication
- Stale/fresh states
- Background refetch
- Retry with backoff
- Pagination
- Optimistic mutations
- Request cancellation
- Offline/reconnect behavior where appropriate

### Example lifecycle

```text
Cached data exists
      ↓
Show immediately
      ↓
Background refetch
      ↓
Fresh response
      ↓
Cache update
      ↓
UI update
```

---

## Q56. Stale search response overwrites the latest result. How do you prevent it?

This is a race condition.

### Option 1 — AbortController

```js
let controller;

async function search(query) {
  controller?.abort();
  controller = new AbortController();

  const response = await fetch(
    `/api/search?q=${encodeURIComponent(query)}`,
    { signal: controller.signal }
  );

  return response.json();
}
```

### Option 2 — request ID

```text
Current request = 8
Response request = 7
→ ignore response 7
```

### Option 3

Use TanStack Query or a saga operator such as `takeLatest` when those abstractions fit the application.

### Senior answer

> "I make request freshness explicit. Cancellation is ideal when the transport supports it, but I also protect the state update path with request identity so even an already-completed older response cannot overwrite newer state."

---

## Q57. E-commerce cart with multiple updates: React Query / SWR optimistic updates

Use server-state cache as the source for remote state and mutate the cache optimistically.

Conceptual flow:

```text
User clicks +
   ↓
Cancel in-flight query if needed
   ↓
Snapshot previous cache
   ↓
Optimistically update cache
   ↓
Send mutation
   ├── success → reconcile with server response
   └── error   → rollback snapshot + notify user
   ↓
Invalidate/refetch as necessary
```

### Important

If multiple users can modify the same server resource, optimistic client updates cannot guarantee global correctness. The server remains authoritative, and conflict/reconciliation behavior must be defined.

---

# 7. Next.js / Rendering / Hydration

## Q58. CSR vs SSR vs SSG

| Strategy | When generated | Good for |
|---|---|---|
| CSR | Browser | Highly interactive authenticated dashboards |
| SSR / dynamic rendering | Request time | Dynamic SEO-sensitive pages |
| SSG / prerendering | Build time | Mostly static content |

### Senior answer

> "I choose based on data freshness, SEO, interaction level, cost and caching. I don't treat SSR as universally better than CSR."

---

## Q59. SSR vs SSG for sports betting odds

Live odds are highly dynamic.

A reasonable architecture is:

```text
Initial page
   ↓
Server render / dynamic fetch
   ↓
Initial odds snapshot
   ↓
Hydrate
   ↓
WebSocket/SSE stream
   ↓
Live odds updates
```

SSG alone is not appropriate for frequently changing odds because prebuilt HTML can become stale.

### Interview answer

> "For SEO-sensitive event pages, I can use server rendering for the initial page and then use a real-time channel for odds updates. SSG is better for content that changes infrequently or can tolerate regeneration/revalidation."

---

## Q60. What is hydration in Next.js?

Hydration is React attaching event handlers and client behavior to server-generated HTML.

```text
Server
 ↓
HTML
 ↓
Browser
 ↓
React loads
 ↓
Hydration
 ↓
Interactive UI
```

Next.js App Router documentation describes Server Components as the default for pages/layouts and Client Components as the place for state, event handlers, effects and browser APIs. citeturn264643search4

---

## Q61. Why do hydration mismatches happen?

The server and client must produce compatible initial output.

Common causes:

```js
Date.now()
Math.random()
localStorage
window.innerWidth
browser locale/time zone
browser-only APIs
```

Problem example:

```jsx
<div>{Date.now()}</div>
```

Server and client can produce different text.

### Correct principle

Keep the initial rendered output deterministic. Put client-only behavior into an appropriate Client Component/effect, or use a rendering boundary designed for browser-only behavior when necessary.

React 19 improved hydration error reporting to make mismatches easier to diagnose. citeturn264643search0

---

## Q62. What are Server Components?

Server Components render outside the client bundle in a supported server environment.

They are useful for:

- server-side data access
- reducing client JavaScript
- keeping server-only logic on the server
- composing server-rendered UI with interactive Client Components

In Next.js App Router, pages and layouts are Server Components by default, while Client Components are used when state, event handlers, effects or browser APIs are needed. citeturn264643search4

### Important

`"use client"` defines a client boundary. It does not mean "run only after every navigation" or "this is the entire application client side."

Also, `"use server"` is associated with Server Functions/Actions, not a directive meaning "this file is a Server Component." React's documentation explicitly calls out this distinction. citeturn264643search0

---

## Q63. How does Next.js automatic code splitting and SSR work?

Modern Next.js splits code by route/module boundaries and can preload/prefetch according to navigation patterns. Server rendering generates the initial HTML on the server; Client Components are hydrated to become interactive.

Conceptually:

```text
Route request
   ↓
Server rendering / data access
   ↓
HTML + RSC payload
   ↓
Browser
   ↓
Hydrate client boundaries
```

The exact behavior depends on whether you're using the App Router or the older Pages Router.

---

## Q64. How does Next.js handle environment variables?

Current Next.js documentation states that environment variables are loaded from `.env` files and that variables exposed to browser code must use the `NEXT_PUBLIC_` prefix. Those public values are bundled/inlined into client-side JavaScript during build. citeturn264643search2turn264643search7

### Practical interpretation

- `.env.local` → local development overrides / local secrets; usually not committed.
- `.env.production` → values intended for production build environment where the deployment process uses them.
- `NEXT_PUBLIC_*` → safe-to-expose client values only.
- Unprefixed variables → server-side only; never treat them as secrets if you expose them through an API response.

### Important

Never put private API keys or database credentials behind `NEXT_PUBLIC_`.

---

## Q65. `ReactDOM.render()` vs `createRoot()`

React 17-style mounting used:

```js
ReactDOM.render(<App />, root);
```

React 18 introduced:

```js
const root = createRoot(document.getElementById("root"));
root.render(<App />);
```

`createRoot` opts into the modern React 18+ client rendering model, including automatic batching behavior and concurrency-related capabilities.

For server-rendered apps, use the hydration APIs rather than treating `createRoot` as the equivalent of hydrating server HTML.

---

# 8. Browser Rendering, CSS & Performance

## Q66. Explain the browser rendering pipeline.

Simplified:

```text
HTML parsing → DOM
CSS parsing  → CSSOM
      ↓
Style calculation
      ↓
Layout
      ↓
Paint
      ↓
Compositing
      ↓
Screen
```

### Layout

Computes geometry: sizes and positions.

### Paint

Draws pixels for text, backgrounds, borders, shadows and images.

### Compositing

Combines layers into the final frame.

### Debugging

Chrome DevTools → Performance can show:

- Scripting
- Style recalculation
- Layout
- Paint
- Composite
- Long Tasks

---

## Q67. Reflow vs repaint

**Reflow/layout** recalculates geometry.

Examples:

```text
width
height
position
margin/padding
font/layout changes
```

**Repaint** redraws visual appearance without necessarily recalculating geometry.

Examples often include:

```text
color
background
shadow
```

These are broad categories; a real browser may perform multiple invalidation steps depending on the change.

---

## Q68. Why is `transform` preferred for CSS animations?

Properties such as `transform` and `opacity` can often be animated without triggering repeated layout, allowing browsers to handle more work in the compositor.

```css
.box {
  transform: translateX(100px);
}
```

versus:

```css
.box {
  left: 100px;
}
```

### Do not say

> "Transform always uses the GPU."

Better:

> "Transform and opacity are often compositor-friendly because they can avoid repeated layout and, depending on the case, avoid repainting the element's contents."

---

## Q69. How do you determine whether JavaScript, reflow, repaint or compositing causes slowness?

Do not guess.

Use Chrome DevTools Performance recording.

### Investigation

```text
Long scripting task?
        ↓
JavaScript bottleneck

Large Recalculate Style/Layout?
        ↓
Style/layout bottleneck

Large Paint?
        ↓
Painting bottleneck

Large Composite Layers?
        ↓
Compositing/layer issue
```

Correlate the trace with:

- user interaction
- frame rate
- network timing
- React Profiler data

### Senior answer

> "I identify where the main-thread time is actually going, then optimize that phase. A fast API response doesn't guarantee a fast UI if the main thread spends hundreds of milliseconds processing, rendering or painting the result."

---

## Q70. How would you optimize a large list with 10k+ rows?

Layer your response:

1. **Reduce data** — server-side pagination/filtering.
2. **Virtualize** — render only the visible window.
3. **Memoize expensive rows selectively.**
4. **Use stable IDs/props.**
5. **Optimize selectors/derived data.**
6. **Avoid repeated layout or expensive calculations.**
7. **Profile before and after.**

For extremely large lists, a combination of pagination + virtualization is often better than either technique alone.

---

## Q71. What is DOM windowing / virtualization?

Windowing renders only items close to the viewport.

```text
100000 records
       ↓
20–100 DOM rows
```

The data can remain large; the DOM remains small.

### View recycling vs windowing

**Windowing:** controls which views exist in the DOM.

**View recycling:** reuses existing view/DOM instances for different records rather than repeatedly creating/destroying them.

React web applications commonly use virtualization/windowing; recycling is particularly prominent in native rendering systems.

---

## Q72. How can a slow page have fast APIs?

Because API latency is only one part of the critical path.

Other bottlenecks:

- JavaScript execution
- Huge JSON parsing
- React rendering
- DOM size
- style/layout
- paint
- image decoding
- main-thread contention

### Diagnostic sequence

```text
Network
 ↓
CPU / scripting
 ↓
React render
 ↓
Style/layout
 ↓
Paint/composite
```

---

## Q73. Re-render debugging scenario

Use:

1. React DevTools Profiler
2. Identify frequently committing components
3. Inspect why each renders
4. Check state location
5. Check context changes
6. Check selector identity
7. Inspect object/function props
8. Add memoization only where justified

### Common issue

```js
const visibleUsers = users.filter(...);
```

creates a new array every render. If a memoized child receives it, the child can still re-render because the reference changed.

A memoized selector or carefully chosen `useMemo` can address this when the computation/identity actually matters.

---

## Q74. Frontend performance optimization techniques

### Loading

- Code splitting
- Lazy loading
- Compression
- CDN
- Critical resource optimization
- Image optimization

### Runtime

- Virtualization
- Memoization where justified
- State locality
- Efficient data structures
- Web Workers for suitable CPU-heavy work

### Network

- caching
- request deduplication
- debounce/throttle
- pagination
- prefetching where beneficial

### Rendering

- Avoid layout thrashing
- Prefer compositor-friendly animations
- Reduce DOM complexity
- Reserve image/content space

---

# 9. Build Tools, Bundle Optimization & Web Vitals

## Q75. Vite vs Webpack

### Vite

Vite's modern development workflow serves source modules through native ESM-oriented development and pre-bundles dependencies for performance/compatibility. Current Vite documentation says dependency pre-bundling is performed with Rolldown and is a development-time optimization. citeturn665623search0turn665623search1

### Webpack

Webpack is a mature, highly configurable bundler with a large plugin/loader ecosystem.

### Interview answer

> "Vite gives an excellent fast development experience with modern ESM-oriented workflows and a simpler default setup for many applications. Webpack remains highly mature and configurable, especially in ecosystems that rely heavily on custom loaders/plugins. I choose based on project constraints and migration cost rather than saying one is universally better."

---

## Q76. How do you analyze and optimize bundle size?

### Measure

- Bundle analyzer / visualizer
- Build stats
- Chrome Coverage
- Lighthouse
- Network waterfall

### Find

- oversized dependencies
- duplicate packages
- large shared chunks
- unused code
- heavy libraries

### Optimize

- route-level code splitting
- dynamic imports
- tree shaking
- replace oversized libraries where justified
- optimize images/fonts
- avoid shipping server-only code to the client
- cache stable vendor/app chunks

### Example

```jsx
const AdminPage = lazy(() => import("./AdminPage"));
```

### Senior answer

> "I measure first, identify the largest contributors, then reduce initial JavaScript by moving infrequently used code behind route or feature boundaries. I also check that the change improves actual user metrics rather than only making the bundle report look smaller."

---

## Q77. What is tree-shaking? What algorithm is used?

Tree shaking is not a single named graph algorithm such as BFS or DFS.

It relies on static analysis of module imports/exports and dead-code elimination.

Conceptually:

```text
Modules
 ↓
Dependency graph
 ↓
Determine reachable/used exports
 ↓
Mark unused code
 ↓
Dead-code elimination / minification
 ↓
Smaller bundle
```

ES Modules help because imports/exports are statically analyzable.

### Important

Side effects can prevent removal of code. A bundler cannot safely eliminate code if executing its module has observable side effects.

---

## Q78. What are Core Web Vitals?

The current Core Web Vitals are:

- **LCP** — Largest Contentful Paint: loading performance
- **INP** — Interaction to Next Paint: responsiveness
- **CLS** — Cumulative Layout Shift: visual stability

### Typical "good" thresholds

- LCP ≤ 2.5s
- INP ≤ 200ms
- CLS ≤ 0.1

### How to improve

**LCP:** server response, critical resource loading, images, CSS/JS.

**INP:** long JS tasks, expensive event handlers, excessive re-renders.

**CLS:** reserve layout space, dimensions for images, avoid unexpected insertion.

### Senior point

Use real-user data when available; Lighthouse is useful for lab diagnosis but does not replace real-user measurements.

---

# 10. Accessibility / WCAG

## Q79. What is WCAG?

WCAG stands for Web Content Accessibility Guidelines. A useful mental model is **POUR**:

```text
Perceivable
Operable
Understandable
Robust
```

### Examples

**Perceivable:** alt text, captions, contrast.

**Operable:** keyboard access, focus management.

**Understandable:** clear labels, consistent behavior.

**Robust:** works with assistive technology and user agents.

WCAG 2.2 is the current W3C accessibility recommendation in the official documentation used for this guide. citeturn665623search3

---

## Q80. Semantic HTML

Prefer:

```html
<button>Save</button>
<nav>...</nav>
<main>...</main>
<article>...</article>
```

instead of replacing native semantics with generic `div` elements.

Semantic HTML provides built-in browser and assistive-technology behavior and often reduces the amount of ARIA you need.

---

## Q81. Keyboard accessibility

Every interactive control should be operable via keyboard.

Examples:

- Tab navigation
- Enter/Space activation
- Escape to close dialogs when expected
- Visible focus
- No keyboard traps

Prefer native `<button>`, `<input>`, `<select>` and links where appropriate.

---

## Q82. Screen readers and ARIA

Use semantic HTML first. Use ARIA when native semantics do not express the behavior sufficiently.

Examples:

```jsx
<button aria-label="Close dialog">×</button>
```

Don't add ARIA to make an incorrectly implemented `div` behave like a button when using a real `<button>` would solve the problem more reliably.

---

## Q83. Focus management

Important for:

- Modal dialogs
- Menus
- SPA route transitions
- Validation errors

For a dialog, a good implementation may:

1. Move focus into the dialog.
2. Keep keyboard navigation inside the dialog if appropriate.
3. Restore focus to the trigger when it closes.

---

## Q84. WCAG contrast requirement

For WCAG 2.2 Level AA, normal text generally requires at least **4.5:1** contrast against the background, while large text generally requires **3:1**. citeturn665623search3turn665623search6

Also ensure:

- meaning is not conveyed by color alone
- focus indicators are visible
- disabled states remain understandable

---

## Q85. Responsive readability / reduced motion

### Readability

- Text should remain readable at increased zoom/text size.
- Avoid layouts that break when text grows.
- Don't bake essential text into images.

WCAG 2.2 includes a Level AA requirement around resizing text up to 200% without loss of content/functionality. citeturn665623search3

### Reduced motion

Respect:

```css
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

Use carefully; don't blindly disable every visual cue if it harms usability.

---

## Q86. Accessible forms and live regions

### Forms

Use explicit labels:

```html
<label for="email">Email</label>
<input id="email" name="email" />
```

Associate errors with fields and expose validation state clearly.

### Live regions

For dynamically updated status messages:

```html
<div aria-live="polite">
  Saved successfully.
</div>
```

Use assertive announcements only when appropriate.

---

## Q87. Accessibility testing strategy

Use a combination of:

- automated checks (axe/Lighthouse-like tooling)
- keyboard-only testing
- browser inspection
- screen-reader testing
- component tests
- end-to-end workflows

### Senior answer

> "Automated accessibility testing catches known technical violations, but it cannot fully assess whether a workflow is understandable or operable. I therefore combine automation with keyboard and assistive-technology testing."

---

# 11. Testing

## Q88. How do you plan unit tests for a new feature?

Start with acceptance criteria and user behavior.

```text
Requirement
 ↓
Acceptance criteria
 ↓
Unit-testable logic
 ↓
Component/integration behavior
 ↓
Critical E2E journey
```

For a cart feature, test:

- add item
- remove item
- quantity changes
- empty state
- loading/error states
- API failures
- important accessibility behavior

### Don't test implementation details

Prefer:

> "After clicking Add to Cart, the product appears in the cart"

instead of:

> "setState was called twice"

---

## Q89. Unit vs Integration vs E2E

### Unit

Small isolated logic:

```text
calculateTotal()
```

### Integration

Multiple pieces working together:

```text
Form → validation → API → UI
```

### E2E

Whole business workflow:

```text
Login → Browse → Add to cart → Checkout
```

Use the smallest test type that gives meaningful protection, while keeping critical journeys covered end to end.

---

## Q90. Jest / React Testing Library testing philosophy

With React Testing Library, test the component from the user's perspective.

Good:

```js
expect(screen.getByRole("button", { name: /save/i })).toBeEnabled();
```

rather than asserting internal state variables or component implementation details.

Mock boundaries such as network services carefully; avoid turning every test into a fully mocked simulation that stops representing real behavior.

---

# 12. Web Security / Authentication / RBAC

## Q91. Authentication implementation in React applications

Separate:

```text
Authentication → Who are you?
Authorization  → What can you do?
```

A common browser architecture:

```text
Login
 ↓
Backend validates credentials/OAuth
 ↓
Session / tokens established
 ↓
Frontend obtains current-user state
 ↓
Protected UI
 ↓
Backend verifies every sensitive request
```

### Important

Frontend route protection is a UX feature, not the security boundary. The backend must authorize access to protected resources.

---

## Q92. JWT flow

Conceptually:

```text
Login
 ↓
Server validates identity
 ↓
Access token / session
 ↓
Browser sends authenticated request
 ↓
Server validates token/session
 ↓
Authorize resource
```

If refresh tokens are used, treat them as high-value credentials and design rotation, expiry, revocation and storage carefully.

---

## Q93. SessionStorage vs LocalStorage

Both are browser storage APIs accessible to JavaScript.

| | localStorage | sessionStorage |
|---|---|---|
| Lifetime | Persists until cleared | Usually tied to page session/tab |
| Sharing | Same origin across tabs/windows depending on browser behavior | Separate per browsing context |
| JS access | Yes | Yes |
| XSS exposure | Yes | Yes |

Do not store high-value credentials there merely because it is convenient.

---

## Q94. Cookie vs browser storage for tokens

### Browser storage risk

If an attacker executes JavaScript through XSS, JavaScript-accessible tokens can potentially be read.

### HttpOnly cookie

An `HttpOnly` cookie cannot be read by normal page JavaScript, reducing direct token theft through many XSS scenarios.

But cookies are automatically sent with requests, so CSRF becomes important depending on the authentication design.

### Common cookie attributes

```text
HttpOnly
Secure
SameSite
```

`SameSite` should be selected based on the application's cross-site requirements.

---

## Q95. XSS — what is it and how do you defend against it?

Cross-Site Scripting occurs when attacker-controlled content is interpreted as executable markup/script.

### Stored XSS

Payload is persisted somewhere such as a database.

### Reflected XSS

Payload comes through a request and is reflected into a response.

### DOM-based XSS

Client-side code creates the vulnerability through unsafe DOM operations.

### React safety

Normal interpolation is escaped:

```jsx
<div>{userInput}</div>
```

Potentially dangerous:

```jsx
dangerouslySetInnerHTML={{ __html: userInput }}
```

### Defense-in-depth

- Output escaping
- Safe templating
- HTML sanitization when raw HTML is truly required
- CSP
- Avoid unsafe DOM APIs
- Secure token handling
- Dependency hygiene

---

## Q96. CORS: Postman works, browser fails

CORS is a browser-enforced security mechanism.

Postman is not subject to browser same-origin enforcement in the same way.

### Preflight

The browser may issue an `OPTIONS` request before the actual request for cross-origin requests that don't meet the conditions of a simple request, such as some combinations of methods/headers/content types.

The server responds with headers such as:

```text
Access-Control-Allow-Origin
Access-Control-Allow-Methods
Access-Control-Allow-Headers
```

### What can frontend control?

The frontend can control its request method, headers and credentials settings within the application's needs, but **the frontend cannot bypass browser CORS enforcement**. The server must return appropriate CORS policy headers.

---

## Q97. RBAC / protected routes

A clean approach:

```text
AuthProvider / Store
       ↓
Current user
       ↓
Route guard / layout
       ↓
Role check
       ↓
Protected UI
```

Example:

```jsx
function ProtectedRoute({ allowedRoles, children }) {
  const { user, loading } = useAuth();

  if (loading) return <Spinner />;
  if (!user) return <Navigate to="/login" />;

  if (!allowedRoles.includes(user.role)) {
    return <Navigate to="/forbidden" />;
  }

  return children;
}
```

### Security rule

Never rely only on this. The backend must repeat authorization checks.

---

## Q98. Secure Express route

Example middleware structure:

```js
app.get(
  "/api/admin/users",
  authenticate,
  authorize("admin"),
  getUsers
);
```

```js
function authenticate(req, res, next) {
  const token = extractToken(req);

  if (!token) {
    return res.status(401).json({
      message: "Unauthorized"
    });
  }

  try {
    req.user = verifyToken(token);
    next();
  } catch {
    return res.status(401).json({
      message: "Invalid token"
    });
  }
}

function authorize(role) {
  return (req, res, next) => {
    if (req.user?.role !== role) {
      return res.status(403).json({
        message: "Forbidden"
      });
    }

    next();
  };
}
```

Add defense in depth:

- HTTPS
- input validation
- secure cookies where appropriate
- CSRF protection where required
- rate limiting
- security headers
- parameterized database queries
- correct CORS
- centralized error handling
- careful logs

---

## Q99. 401 vs 403

```text
401 → authentication is missing/invalid
403 → request is understood but access is forbidden
```

A logged-in user without admin rights may receive 403.

---

# 13. API Strategy, Caching, Retries, Rate Limits & BFF

## Q100. API handling architecture

Avoid scattering networking code in every component.

Prefer:

```text
Component
 ↓
Hook / feature service
 ↓
API client
 ↓
HTTP layer
 ↓
Backend
```

Centralize:

- base URL/config
- auth/session behavior
- serialization
- standard errors
- telemetry
- retries where safe

---

## Q101. Handling API rate limits gracefully

When the server returns `429`:

1. Respect `Retry-After` when provided.
2. Use bounded exponential backoff with jitter where retrying is safe.
3. Deduplicate requests.
4. Cache data.
5. Debounce search and throttle high-frequency events.
6. Queue requests if appropriate.
7. Don't blindly retry non-transient errors.

Example retry intervals conceptually:

```text
1s → 2s → 4s → 8s → stop
```

### Senior answer

> "Rate-limit handling is not just retrying 429s. I reduce unnecessary traffic first through caching, deduplication and controlled concurrency, then apply bounded retry behavior for transient failures."

---

## Q102. BFF architecture

BFF = Backend-for-Frontend.

```text
React / Next.js
      ↓
     BFF
   /  |  \
svc svc svc
```

The BFF can:

- Aggregate multiple services
- Shape frontend-specific payloads
- Handle authentication/session integration
- Centralize caching
- Hide internal service topology
- Reduce round trips

### Example

A product page needs:

```text
product
pricing
inventory
reviews
recommendations
```

Instead of five browser requests:

```text
Browser → BFF → five backend services
```

The browser can make one frontend-oriented request.

### Trade-offs

- Additional service
- Operational complexity
- Potential bottleneck
- Need for clear ownership

---

## Q103. gRPC vs JSON / REST

gRPC commonly uses Protocol Buffers (binary serialization) over HTTP/2 and supports streaming and strongly defined contracts.

JSON APIs are human-readable and generally simpler for public browser APIs.

### Why gRPC can be efficient

- Compact binary encoding
- Fast serialization/deserialization
- Strong schema
- HTTP/2 capabilities
- Streaming

### Browser nuance

Direct browser use often involves **gRPC-Web** or a server/BFF layer rather than arbitrary native gRPC access.

### Interview answer

> "For internal service-to-service communication where latency, bandwidth and typed contracts matter, gRPC can be a strong choice. For public browser APIs, REST/JSON can remain simpler and more interoperable."

---

## Q104. SSE vs WebSockets

| | SSE | WebSocket |
|---|---|---|
| Direction | Server → client | Bidirectional |
| Transport | HTTP-based event stream | WebSocket protocol |
| Best for | Server push | Interactive real-time communication |
| Complexity | Lower | Higher |

### SSE examples

- live notifications
- job progress
- order status
- server-pushed updates

### WebSocket examples

- chat
- collaborative editing
- games
- live bidirectional trading/betting interactions

### Interview answer

> "If only the server needs to push updates, SSE is often simpler. If both sides need low-latency bidirectional communication, I'd choose WebSockets."

---

## Q105. API caching, retries and background sync

Use a cache layer that knows the difference between:

```text
fresh
stale
loading
error
invalidated
```

For retries:

```text
transient error → bounded retry
permanent error → fail fast
```

For offline/background sync, a service worker and appropriate data synchronization strategy may be useful, but conflict resolution and security must be explicitly designed.

---

# 14. Angular / RxJS / Node.js / Express

## Q106. Dependency Injection in Angular

Dependency Injection means a component/service receives dependencies rather than creating them internally.

Without DI:

```ts
class UserService {
  api = new ApiService();
}
```

With DI conceptually:

```ts
class UserService {
  constructor(private api: ApiService) {}
}
```

Angular's injector resolves the dependency according to the provider configuration and scope.

### Honest answer for a React developer

> "My primary production experience is React, but I understand Angular's DI model: Angular's injector constructs and provides services according to providers and scopes, which reduces coupling and improves testability."

---

## Q107. Standalone Components vs NgModules

Traditional Angular:

```ts
@NgModule({
  declarations: [UserComponent],
  imports: [CommonModule]
})
class UserModule {}
```

Standalone component:

```ts
@Component({
  standalone: true,
  imports: [CommonModule],
  template: `...`
})
class UserComponent {}
```

Standalone APIs reduce module boilerplate and make dependency ownership/lazy-loading boundaries more direct.

---

## Q108. What is Angular Async Pipe?

The `async` pipe subscribes to an Observable/Promise in a template, displays emitted values, and handles subscription cleanup for the template binding.

Example:

```html
<div>{{ user$ | async }}</div>
```

### React equivalent?

There is no exact equivalent. In React, the same concerns are usually handled through hooks or server-state/data libraries.

---

## Q109. What is `process.nextTick()`?

Node.js-specific API.

```js
console.log("A");

process.nextTick(() => {
  console.log("B");
});

console.log("C");
```

Output:

```text
A
C
B
```

`process.nextTick()` schedules work to run after the current operation and before the Node event loop proceeds to later phases. Excessive recursive use can starve the event loop.

### Don't equate it with

```js
setTimeout(fn, 0)
```

They have different scheduling semantics in Node.

---

## Q110. What are Node.js Buffers?

`Buffer` represents raw binary data.

```js
const buffer = Buffer.from("Hello");
console.log(buffer);
```

Useful for:

- files
- streams
- sockets
- binary protocols
- encryption
- image/audio processing

---

# 15. CI/CD / GitHub Actions

## Q111. What is GitHub Actions?

GitHub Actions is a CI/CD automation platform integrated with GitHub. Workflows are YAML definitions triggered by events such as pushes and pull requests, and contain jobs/steps running on GitHub-hosted or self-hosted runners. citeturn665623search2turn665623search4

### Typical frontend workflow

```text
Pull Request
   ↓
lint
   ↓
type-check
   ↓
unit tests
   ↓
build
   ↓
review/merge
   ↓
staging deploy
   ↓
smoke tests
   ↓
production
```

---

## Q112. Example GitHub Actions workflow

```yaml
name: Frontend CI

on:
  pull_request:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4

      - uses: actions/setup-node@v4
        with:
          node-version: 20

      - run: npm ci
      - run: npm run lint
      - run: npm run test
      - run: npm run build
```

### Security

Use GitHub Secrets or an appropriate secret manager. Do not hard-code private credentials in workflow files.

---

## Q113. CI vs CD

### Continuous Integration

Validate changes automatically:

```text
commit
 ↓
lint
 ↓
test
 ↓
build
```

### Continuous Delivery

Code is continuously prepared and can be released, often with a production approval step.

### Continuous Deployment

Validated changes are automatically deployed to production.

---

# 16. SEO

## Q114. What is SEO from a frontend perspective?

SEO is not just meta tags. It includes:

- Crawlable semantic content
- Metadata
- Correct headings
- Internal linking
- Canonical URLs
- Structured data where applicable
- Performance/user experience
- Correct indexation controls
- Server/pre-rendered HTML when appropriate

---

## Q115. SSR and SEO benefits

SSR can make meaningful HTML available in the initial response instead of depending entirely on client-side rendering.

Useful for:

- product pages
- article pages
- public landing pages
- dynamic pages where SEO matters

SSR isn't automatically better for every route. Internal dashboards usually don't need indexing and can often use CSR/client-heavy rendering.

---

## Q116. SEO with Next.js

Consider:

- Metadata API / page metadata
- Semantic HTML
- sitemap
- robots.txt
- canonical URLs
- structured data where relevant
- image optimization
- correct status codes
- stable content URLs
- SSR/SSG/revalidation depending on content

---

# 17. Frontend Architecture & Scalability

## Q117. How would you design a scalable React app with 100+ pages?

Prefer feature/domain-oriented organization:

```text
src/
├── app/
│   ├── routes/
│   ├── providers/
│   └── config/
├── features/
│   ├── auth/
│   ├── dashboard/
│   ├── users/
│   ├── reports/
│   └── payments/
├── components/
├── services/
├── store/
├── hooks/
└── utils/
```

### Layer responsibilities

**App:** composition and routing.

**Features:** domain logic.

**Components:** reusable UI primitives.

**Services:** API/external integrations.

**Store:** truly global client state.

### Rendering strategy

Use route-level code splitting and lazy load heavy feature modules.

### State strategy

```text
UI state → local state
Client cross-feature state → Redux/Context/etc.
Server state → TanStack Query/SWR/etc.
```

---

## Q118. Component system design / reusable component architecture

A component library should separate:

```text
Design tokens
 ↓
Primitives
 ↓
Composite components
 ↓
Feature/business components
```

Examples:

```text
Button
Input
Modal
Dropdown
Table
DatePicker
```

Business components should compose these primitives instead of reinventing interaction behavior.

---

## Q119. Build a component library used by multiple teams

Important dimensions:

### API design

Stable, discoverable props.

### Accessibility

Keyboard, focus, semantic behavior.

### Theming

Design tokens for color, spacing, typography, radius etc.

### Documentation

Storybook or equivalent documentation system.

### Testing

Unit, interaction, accessibility and visual regression where appropriate.

### Versioning

Semantic versioning and a clear migration/deprecation policy.

### Governance

Prevent duplicate components and uncontrolled divergence across teams.

### Senior answer

> "The hard part is not publishing Button and Modal. The hard part is creating stable contracts and governance so multiple teams don't create incompatible variants of the same component."

---

## Q120. Cross-platform compatibility

Consider:

- Browser support matrix
- Mobile vs desktop interaction
- Touch vs mouse vs keyboard
- Responsive layout
- Feature detection / progressive enhancement
- Polyfills only when required
- Testing on target browsers/devices

Don't solve compatibility by blindly adding dependencies. First determine the actual supported browser/device set.

---

## Q121. Frontend architecture for 1M+ daily users

Treat this as a distributed system problem:

```text
CDN
 ↓
Browser
 ↓
Frontend / Next.js
 ↓
BFF/API
 ↓
Services
 ↓
Databases/caches
```

### Frontend

- small initial bundle
- route/feature code splitting
- caching
- image optimization
- virtualization
- efficient rendering

### Platform

- CDN
- horizontal service scaling
- caching
- rate limiting
- observability
- feature flags
- graceful degradation

### Metrics

- LCP
- INP
- CLS
- JS errors
- API latency
- API error rate
- business funnel metrics

### Senior answer

> "The user count changes how I think about capacity, but it does not mean React itself should contain 1M-user logic. I need to distribute static assets, cache aggressively, keep the client efficient, make backend services scalable, and build observability around the real bottlenecks."

---

## Q122. Architecture & scalability — decision framework

For any frontend architecture problem ask:

```text
Who are the users?
How much data?
What changes frequently?
What must be realtime?
SEO?
Latency target?
Offline requirement?
Security boundary?
Team size?
Deployment model?
```

Then choose:

- rendering strategy
- state strategy
- API strategy
- caching
- component boundaries
- code-splitting boundaries
- observability

---

# 18. Frontend System Design

## Q123. Design a Pinterest-like Grid UI

### Requirements

Clarify:

- variable-height images?
- infinite scrolling?
- SEO?
- filtering/search?
- expected dataset size?
- logged-in features?

### Architecture

```text
Browser
  ↓
Next.js/React
  ├── Search
  ├── Filters
  └── MasonryGrid
       └── PinCard
            └── Image
  ↓
Query/cache layer
  ↓
BFF/API
  ↓
Pin/Search/User services
  ↓
DB

Images → CDN
```

### Data

Prefer cursor-based pagination for dynamic feeds:

```http
GET /api/pins?cursor=abc&limit=30
```

Response:

```json
{
  "items": [],
  "nextCursor": "xyz",
  "hasMore": true
}
```

### Infinite scroll

Use `IntersectionObserver` on a sentinel.

### Performance

- lazy-load images
- responsive image sizes
- CDN resizing
- reserve image dimensions to avoid CLS
- virtualization where practical
- query caching

### Error handling

Don't destroy the entire feed when page 5 fails. Show existing content and a retry affordance.

---

## Q124. Design a real-time collaborative text editor like Google Docs

### Core challenge

Multiple users edit the same logical document simultaneously.

Naïve last-write-wins would cause lost updates.

### Architecture

```text
Client A ─┐
Client B ─┼→ WebSocket gateway → Collaboration service
Client C ─┘                       ↓
                                Document state
                                   ↓
                              Persistence
```

### Synchronization algorithms

Common conceptual approaches:

- Operational Transformation (OT)
- Conflict-free Replicated Data Types (CRDTs)

The choice depends on consistency model, implementation complexity, offline support and library ecosystem.

### Client

```text
Editor state
 ↓
Local operation
 ↓
Optimistic local apply
 ↓
Send operation
 ↓
Server ordering / transformation
 ↓
Broadcast remote ops
 ↓
Merge
```

### Important NFRs

- low latency
- conflict resolution
- reconnection
- offline editing if required
- persistence
- presence/cursors
- authorization
- document history

---

## Q125. Design a rate limiter for API calls in a SPA

### Client-side purpose

Protect the browser from excessive calls and improve UX.

Use:

```text
debounce
throttle
request deduplication
queue
cache
concurrency limit
```

### Example

For search:

```text
Typing
 ↓
debounce 300ms
 ↓
request
```

For scroll analytics:

```text
many events
 ↓
throttle
 ↓
controlled calls
```

### Important

Client rate limiting does **not** replace server-side rate limiting. The backend must enforce security and capacity boundaries.

---

## Q126. Design dynamic pagination / infinite scrolling

### Preferred flow

```text
Initial page
 ↓
items + nextCursor
 ↓
IntersectionObserver
 ↓
fetch next cursor
 ↓
append
 ↓
repeat
```

### Why cursor pagination?

It behaves better than offsets when a feed changes between requests.

### Important edge cases

- duplicate items
- new items inserted at top
- request racing
- retrying a failed page
- maintaining scroll position
- empty result
- end of feed
- offline/reconnect

---

## Q127. Design a client-side state management system like Redux Toolkit

### Requirements

- immutable-looking updates
- predictable dispatching
- selectors
- middleware
- devtools
- persistence if required
- subscriptions

### Architecture

```text
UI
 ↓
dispatch(action)
 ↓
middleware
 ↓
reducer
 ↓
store
 ↓
selector
 ↓
UI
```

### Example slice concept

```js
const counterSlice = createSlice({
  name: "counter",
  initialState: { value: 0 },
  reducers: {
    increment(state) {
      state.value += 1;
    }
  }
});
```

RTK uses Immer internally to provide a mutable-looking reducer syntax while producing immutable state updates.

### Important design rules

- Keep source of truth clear.
- Store normalized entities when appropriate.
- Keep selectors close to state semantics.
- Separate server state from client state where possible.

---

## Q128. Design social login / OAuth / JWT authentication flow

### High-level

```text
User
 ↓
Frontend
 ↓
OAuth provider
 ↓
Authorization code
 ↓
Backend callback
 ↓
Exchange code securely
 ↓
Create application session
 ↓
Browser receives secure session cookie
 ↓
Authenticated requests
```

### Why Authorization Code flow?

For web applications, the Authorization Code flow is generally preferred over exposing provider secrets to the browser. With public clients, PKCE provides protection for authorization code interception and is commonly used.

### Session vs JWT

A system can use:

- opaque server sessions
- access/refresh token architecture
- signed JWTs

JWT is a token format, not an authentication architecture by itself.

### Security

- HTTPS
- state/nonce protection where appropriate
- PKCE for applicable public clients
- secure cookies/session storage strategy
- CSRF considerations
- token expiry/rotation
- backend authorization

---

## Q129. Design a scalable notification system

### Requirements

- millions of users
- real-time notifications
- unread count
- persistence
- retry
- preference settings
- multi-device

### Architecture

```text
Event producers
     ↓
Message broker / event bus
     ↓
Notification service
   ├── persistence
   ├── preference filtering
   └── delivery
       ├── WebSocket/SSE
       ├── Push/email/etc.
       └── retry queue
     ↓
Client
     ↓
Notification cache/state
```

### Client

- initial notification fetch
- real-time stream
- dedup by notification ID
- optimistic read/unread updates if safe
- reconnect logic
- backfill missed notifications after reconnect

### Scalability

- partition by user/tenant where appropriate
- horizontally scale connection gateways
- broker events
- cache unread counts carefully
- avoid broadcasting every event to every client

---

# 19. Coding Appendix

## C1. Implement `chunk<T>(items, size)`

```ts
function chunk<T>(items: T[], size: number): T[][] {
  if (size <= 0) {
    throw new Error("size must be greater than 0");
  }

  const result: T[][] = [];

  for (let i = 0; i < items.length; i += size) {
    result.push(items.slice(i, i + size));
  }

  return result;
}
```

### Complexity

```text
Time: O(n)
Space: O(n)
```

### Why not `splice()`?

Because `splice()` mutates the source array.

---

## C2. Find first unique character — HashMap pattern

```js
function firstUnique(str) {
  const frequency = new Map();

  for (const char of str) {
    frequency.set(
      char,
      (frequency.get(char) || 0) + 1
    );
  }

  for (const char of str) {
    if (frequency.get(char) === 1) {
      return char;
    }
  }

  return null;
}
```

Complexity:

```text
Time: O(n)
Space: O(k)
```

---

## C3. Flatten a nested array

### Recursive

```js
function flatten(arr) {
  const result = [];

  for (const item of arr) {
    if (Array.isArray(item)) {
      result.push(...flatten(item));
    } else {
      result.push(item);
    }
  }

  return result;
}
```

### Iterative alternative

```js
function flatten(arr) {
  const stack = [...arr];
  const result = [];

  while (stack.length) {
    const item = stack.pop();

    if (Array.isArray(item)) {
      stack.push(...item);
    } else {
      result.push(item);
    }
  }

  return result.reverse();
}
```

Be ready to discuss recursion depth and complexity.

---

## C4. Top-K Elements

### Simple solution

```js
function topK(nums, k) {
  return [...nums]
    .sort((a, b) => b - a)
    .slice(0, k);
}
```

Complexity:

```text
O(n log n)
```

### Senior improvement

For very large `n` and small `k`, maintain a min-heap of size `k`:

```text
O(n log k)
```

This is the important trade-off to mention if the interviewer pushes on scale.

---

## C5. Expand / collapse React list

```jsx
function ExpandableList({ items }) {
  const [expandedId, setExpandedId] = useState(null);

  function toggle(id) {
    setExpandedId(prev => (
      prev === id ? null : id
    ));
  }

  return (
    <ul>
      {items.map(item => {
        const expanded = expandedId === item.id;

        return (
          <li key={item.id}>
            <button
              type="button"
              aria-expanded={expanded}
              aria-controls={`content-${item.id}`}
              onClick={() => toggle(item.id)}
            >
              {item.title}
            </button>

            {expanded && (
              <div id={`content-${item.id}`}>
                {item.content}
              </div>
            )}
          </li>
        );
      })}
    </ul>
  );
}
```

### Follow-up

If multiple rows can be expanded simultaneously, use a `Set` of IDs or another normalized structure rather than a single `expandedId`.

---

## C6. Reusable Button with variants and sizes

```tsx
type ButtonVariant = "primary" | "secondary" | "danger";
type ButtonSize = "sm" | "md" | "lg";

type ButtonProps = {
  variant?: ButtonVariant;
  size?: ButtonSize;
  children: React.ReactNode;
  disabled?: boolean;
  loading?: boolean;
  type?: "button" | "submit" | "reset";
  onClick?: React.MouseEventHandler<HTMLButtonElement>;
};

function Button({
  variant = "primary",
  size = "md",
  children,
  disabled = false,
  loading = false,
  type = "button",
  onClick
}: ButtonProps) {
  return (
    <button
      type={type}
      disabled={disabled || loading}
      aria-busy={loading}
      className={`button button-${variant} button-${size}`}
      onClick={onClick}
    >
      {loading ? "Loading..." : children}
    </button>
  );
}
```

### Senior follow-ups

- forward/pass ref capability as required by the library's React version
- focus states
- keyboard behavior
- loading semantics
- design tokens
- accessibility tests
- visual regression

---

## C7. Searchable multi-select dropdown

```jsx
function MultiSelect({ options, value, onChange }) {
  const [open, setOpen] = useState(false);
  const [query, setQuery] = useState("");

  const filtered = options.filter(option =>
    option.label.toLowerCase().includes(query.toLowerCase())
  );

  function toggleOption(option) {
    const exists = value.some(item => item.id === option.id);

    if (exists) {
      onChange(
        value.filter(item => item.id !== option.id)
      );
    } else {
      onChange([...value, option]);
    }
  }

  return (
    <div className="multi-select">
      <button
        type="button"
        aria-expanded={open}
        onClick={() => setOpen(prev => !prev)}
      >
        {value.length
          ? `${value.length} selected`
          : "Select"}
      </button>

      {open && (
        <div role="dialog">
          <input
            value={query}
            onChange={e => setQuery(e.target.value)}
            placeholder="Search"
          />

          {filtered.map(option => (
            <label key={option.id}>
              <input
                type="checkbox"
                checked={value.some(v => v.id === option.id)}
                onChange={() => toggleOption(option)}
              />
              {option.label}
            </label>
          ))}
        </div>
      )}
    </div>
  );
}
```

### Production considerations

- keyboard navigation
- focus management
- Escape-to-close
- async/server search
- virtualization for huge option sets
- click-outside handling
- ARIA semantics appropriate to the actual widget pattern
- selection limits
- loading/error states

---

## C8. Promise polyfill — interview-grade core implementation

> This is an educational core implementation, not a full reproduction of the ECMAScript Promise Resolution Procedure.

```js
function MyPromise(executor) {
  if (typeof executor !== "function") {
    throw new TypeError("Executor must be a function");
  }

  this.state = "pending";
  this.value = undefined;
  this.handlers = [];

  const fulfill = value => {
    if (this.state !== "pending") return;

    this.state = "fulfilled";
    this.value = value;

    this.handlers.forEach(handle);
    this.handlers = [];
  };

  const reject = reason => {
    if (this.state !== "pending") return;

    this.state = "rejected";
    this.value = reason;

    this.handlers.forEach(handle);
    this.handlers = [];
  };

  const resolve = value => {
    if (this.state !== "pending") return;

    if (
      value !== null &&
      (typeof value === "object" || typeof value === "function")
    ) {
      let then;

      try {
        then = value.then;
      } catch (error) {
        reject(error);
        return;
      }

      if (typeof then === "function") {
        let called = false;

        try {
          then.call(
            value,
            nextValue => {
              if (called) return;
              called = true;
              resolve(nextValue);
            },
            reason => {
              if (called) return;
              called = true;
              reject(reason);
            }
          );
        } catch (error) {
          if (!called) reject(error);
        }

        return;
      }
    }

    fulfill(value);
  };

  const handle = handler => {
    if (this.state === "pending") {
      this.handlers.push(handler);
      return;
    }

    setTimeout(() => {
      const callback =
        this.state === "fulfilled"
          ? handler.onFulfilled
          : handler.onRejected;

      if (typeof callback !== "function") {
        const fallback =
          this.state === "fulfilled"
            ? handler.resolve
            : handler.reject;

        fallback(this.value);
        return;
      }

      try {
        const result = callback(this.value);
        handler.resolve(result);
      } catch (error) {
        handler.reject(error);
      }
    }, 0);
  };

  this.then = (onFulfilled, onRejected) => {
    return new MyPromise((resolveNext, rejectNext) => {
      handle({
        onFulfilled,
        onRejected,
        resolve: resolveNext,
        reject: rejectNext
      });
    });
  };

  this.catch = onRejected => this.then(null, onRejected);

  try {
    executor(resolve, reject);
  } catch (error) {
    reject(error);
  }
}
```

### What the interviewer is checking

- State machine
- Resolve/reject only once
- Thenable adoption
- Chaining
- Error propagation
- Returning a new Promise from `.then()`
- Asynchronous continuation semantics

---

## C9. Async scheduler with maximum concurrency

```js
class Scheduler {
  constructor(limit) {
    if (limit <= 0) {
      throw new Error("limit must be greater than 0");
    }

    this.limit = limit;
    this.running = 0;
    this.queue = [];
  }

  add(task) {
    return new Promise((resolve, reject) => {
      this.queue.push({ task, resolve, reject });
      this.runNext();
    });
  }

  runNext() {
    while (
      this.running < this.limit &&
      this.queue.length
    ) {
      const { task, resolve, reject } = this.queue.shift();

      this.running += 1;

      Promise.resolve()
        .then(task)
        .then(resolve, reject)
        .finally(() => {
          this.running -= 1;
          this.runNext();
        });
    }
  }
}
```

### Core invariant

```text
running <= concurrencyLimit
```

### Follow-up

Be ready to discuss cancellation, prioritization, retries, timeouts and fair scheduling.

---

## C10. React-like Class Component from ES5 concepts

A simplified educational abstraction:

```js
function Component(props) {
  this.props = props || {};
  this.state = {};
  this._container = null;
}

Component.prototype.setState = function (partialState) {
  this.state = Object.assign(
    {},
    this.state,
    typeof partialState === "function"
      ? partialState(this.state, this.props)
      : partialState
  );

  this.update();
};

Component.prototype.update = function () {
  const nextNode = this.render();

  this._container.innerHTML = "";
  this._container.appendChild(nextNode);
};
```

A derived component can inherit with:

```js
Counter.prototype = Object.create(Component.prototype);
Counter.prototype.constructor = Counter;
```

### Important disclaimer

Real React is far more sophisticated. This coding exercise is meant to demonstrate understanding of prototypes, state, render/update flow and lifecycle-style abstractions.

---

# 20. Managerial / Behavioral / STAR Answers

## Q130. Critical production bug broke the UI

### STAR answer

**Situation**

> "We had a production issue where a key UI flow stopped behaving correctly because the frontend encountered an unexpected data/state condition."

**Task**

> "My first priority was to restore the user flow safely while determining the root cause so we didn't create another issue."

**Action**

> "I reproduced the problem, checked the browser console and network requests, compared the failing path with a working path, and reviewed recent changes. Once I identified the failing condition, I fixed it, tested the affected flow and related edge cases, and verified the deployment. I also added or improved regression coverage around the failure mode."

**Result**

> "The production flow was restored, and the regression protection reduced the chance of the same class of issue recurring."

### Important

Replace this with your real incident. Do not invent outage duration, customer counts or percentage improvements.

---

## Q131. How do you prioritize technical debt vs new features?

### Answer

> "I prioritize debt based on business impact, risk and cost of delay. Security, data integrity and production reliability issues come before lower-risk feature work. Debt that significantly slows feature delivery or creates repeated incidents is also worth prioritizing. Lower-risk refactoring can be scheduled incrementally so it doesn't disappear behind feature work."

A useful mental model:

```text
Security / correctness
        ↓
Production stability
        ↓
Developer productivity / scalability
        ↓
Maintainability improvements
        ↓
Nice-to-have refactoring
```

Do not turn this into a rigid universal ordering; context matters.

---

## Q132. Conflict with backend team

### Answer

> "I try to frame disagreements around the API contract and user impact rather than around teams. First I understand the backend constraint, then I explain what the frontend needs and why, and we compare alternatives. If a breaking change is unavoidable, I'd prefer versioning, backward compatibility or a coordinated rollout instead of silently breaking the existing client."

### Example

Frontend needs:

```json
{
  "items": [],
  "total": 1000,
  "nextCursor": "..."
}
```

If backend changes the shape, discuss the contract instead of saying "backend is wrong."

---

## Q133. Conflict with designers

### Answer

> "I first make sure I understand the design goal and user problem. If the exact implementation is technically expensive, inaccessible or incompatible with platform behavior, I explain the constraint and propose alternatives that preserve the intended user outcome. I prefer resolving differences with concrete prototypes, browser behavior or measured evidence rather than opinion."

---

## Q134. How do you communicate complex technical decisions to non-technical stakeholders?

Use:

```text
Business problem
 ↓
Options
 ↓
Trade-offs
 ↓
Recommendation
 ↓
Expected impact
 ↓
Risks / next steps
```

### Example

Instead of:

> "We're going to implement dynamic imports with route-level Suspense boundaries."

Say:

> "The application currently downloads code for features the user may never open. We'll change the loading strategy so large features load when they are needed, reducing the initial download and improving the first-use experience."

---

## Q135. How do you handle disagreement with backend/design/QA?

A strong pattern:

1. Restate the shared goal.
2. Separate facts from assumptions.
3. Identify constraints.
4. Compare options.
5. Make the decision explicit.
6. Record the contract/decision if important.
7. Follow up based on outcomes.

This demonstrates collaboration rather than avoidance of conflict.

---

## Q136. How do you communicate a performance optimization?

Use business language first:

> "The main issue was that users were downloading and executing code for features they weren't using. We moved heavy features behind lazy-loaded boundaries and reduced work during initial load. We then validated the change with browser performance traces and user metrics."

If exact metrics are known, state them. Otherwise don't fabricate numbers.

---

## Q137. Tell me about a time you used Copilot.

### Interview-safe answer

> "I use Copilot primarily as a development assistant rather than as an architectural decision-maker. I've used it to generate repetitive boilerplate, create initial test cases, suggest utility implementations, explain unfamiliar code and explore alternatives. I still review the generated code carefully, especially around security, performance, typing, business logic and API contracts."

### Follow-up: Can Copilot replace developers?

> "I see it as a productivity multiplier. It can accelerate implementation, but the developer still owns requirements, architecture, validation, security and the final code quality."

---

# 21. Project / Experience-Based Senior Answers

## Q138. What performance optimizations have you implemented?

Use only techniques you have actually used or can defend technically.

A good answer based on your project background:

> "I've worked with frontend performance techniques such as lazy loading/code splitting, reducing unnecessary React renders, memoized selectors where appropriate, debounce for user-driven requests, pagination/infinite scrolling, and performance analysis through browser tooling. I also pay attention to Core Web Vitals and bundle size rather than looking at rendering in isolation."

### Stronger follow-up answer

> "One principle I follow is measure first. For example, if a large list is slow, I don't assume `React.memo` is the answer. I first determine whether the bottleneck is excessive rendering, DOM size, data processing, layout or network behavior."

---

## Q139. How did you use Google Tag Manager?

A senior framing:

> "I use GTM to capture meaningful product events such as user journeys, conversions, affiliate-related events or interaction funnels. I try to keep the event model consistent, avoid sending duplicate events, load analytics asynchronously, and validate the data in both the browser and the analytics destination. I also consider the performance cost of analytics scripts and avoid blocking critical UI work."

---

## Q140. Debugging excessive re-renders in a Redux application

### Investigation

```text
React Profiler
 ↓
Find hot component
 ↓
Why did it render?
 ↓
State subscription
Selector identity
Props identity
Context
 ↓
Optimize bottleneck
```

### Typical fixes

- granular selectors
- memoized selectors
- normalized state
- `React.memo` for expensive leaf components
- stable props where identity matters
- move state closer to where it is used

---

# 22. Senior Frontend Architecture: Ten Original Architect-Level Topics

## Q141. Architecture & Scalability

Use this decision framework:

```text
Requirements
 ↓
Boundaries
 ↓
Data ownership
 ↓
State strategy
 ↓
Rendering strategy
 ↓
API strategy
 ↓
Performance
 ↓
Observability
```

### Example architecture

```text
App shell
 ├── Auth
 ├── Routing
 ├── Design system
 └── Feature modules
       ├── Users
       ├── Reports
       └── Dashboard
```

Avoid monolithic components and avoid over-fragmenting tiny components without a stable abstraction.

---

## Q142. Performance Optimization

Start with:

```text
Measure
 ↓
Identify bottleneck
 ↓
Hypothesis
 ↓
Optimize
 ↓
Re-measure
```

Use:

- React Profiler
- browser Performance
- Lighthouse
- bundle analyzer
- real user monitoring

Then optimize loading, runtime, network and rendering separately.

---

## Q143. State Management Strategy

Classify state before choosing tools:

```text
Ephemeral UI state
→ useState/useReducer

Shared client state
→ Context/Redux/etc.

Server state
→ TanStack Query/SWR/etc.

URL state
→ router/search params
```

The most common architecture mistake is storing every kind of state in one global store.

---

## Q144. Component System Design

Design around:

- stable contracts
- composition
- accessibility
- testability
- controlled/uncontrolled patterns where useful
- predictable styling
- versioning

A component becomes reusable when its behavior is stable, not merely when its JSX looks similar to another component.

---

## Q145. Routing & Rendering Strategy

Select routing/rendering based on:

- SEO
- authentication
- data freshness
- interactivity
- initial load
- caching

Use route-level code splitting and avoid loading administrative or low-frequency features on every public page.

---

## Q146. Cross-platform Compatibility

Define target browsers/devices first.

Then validate:

- layout
- touch/keyboard
- input behavior
- responsive breakpoints
- font/rendering differences
- browser APIs
- fallback behavior

Progressive enhancement is often safer than browser-specific hacks.

---

## Q147. Debugging Production Issues

Use observability:

```text
Error tracking
Performance monitoring
Network logs
Console diagnostics
User/session context
Release version
```

A production bug should become easier to diagnose over time through better telemetry and regression tests.

---

## Q148. Frontend Security

Think in layers:

```text
Browser
 ↓
XSS protection
 ↓
Authentication
 ↓
Authorization
 ↓
Transport security
 ↓
API validation
 ↓
Backend security
```

Do not treat the frontend as the final authorization boundary.

---

## Q149. API & Data Strategy

Define:

- data ownership
- API contracts
- caching
- pagination
- retries
- cancellation
- consistency requirements
- error semantics

### Senior question to ask

> "Is this data server-authoritative, and how stale can the UI safely be?"

That question often determines the right client-state architecture.

---

## Q150. Testing Strategy

Use layers:

```text
Unit
 ↓
Integration
 ↓
Critical E2E
```

Also include:

- accessibility
- performance checks where valuable
- visual regression when the design system requires it
- contract/schema tests for API boundaries when appropriate

---

# 23. Additional Interview Questions and Answers from Earlier Lists

## Q151. What is callback hell, and how do you avoid it?

Callback hell is deeply nested callback structure that makes control flow and error handling difficult.

```js
getUser(id, user => {
  getOrders(user, orders => {
    getPayment(orders, payment => {
      // deeply nested
    });
  });
});
```

Use Promises / async-await:

```js
const user = await getUser(id);
const orders = await getOrders(user);
const payment = await getPayment(orders);
```

But don't serialize independent operations unnecessarily; use `Promise.all` when work is independent.

---

## Q152. Promise vs `async/await` when operations are independent

Bad:

```js
const a = await getA();
const b = await getB();
```

if `b` doesn't depend on `a`.

Better:

```js
const [a, b] = await Promise.all([
  getA(),
  getB()
]);
```

This reduces total waiting time by running independent operations concurrently.

---

## Q153. Generators

Generators can pause and resume execution with `yield`.

```js
function* ids() {
  yield 1;
  yield 2;
  yield 3;
}

const iterator = ids();

console.log(iterator.next());
console.log(iterator.next());
```

They are useful for custom iterators and certain control-flow designs. Redux-Saga uses generator functions to describe asynchronous workflows.

---

## Q154. Why use Redux-Saga?

Saga models side effects as generator-driven workflows.

Common effects:

```text
call → invoke async function
put  → dispatch action
takeEvery → handle every occurrence
takeLatest → keep latest workflow
select → read state
```

### Trade-off

Powerful for complex workflows, cancellation and orchestration, but adds abstraction and learning cost compared with simpler approaches.

---

## Q155. API error handling in React

Handle states explicitly:

```text
idle
loading
success
empty
error
```

And classify errors:

```text
401 → re-auth/session flow
403 → forbidden UI
404 → not found
409 → business conflict
429 → rate limit handling
5xx → retry/graceful failure
```

Don't show a generic error for every failure when the UI can give a more useful recovery path.

---

## Q156. How would you implement authentication with Context API?

```jsx
const AuthContext = createContext(null);

function AuthProvider({ children }) {
  const [user, setUser] = useState(null);
  const [loading, setLoading] = useState(true);

  useEffect(() => {
    getCurrentUser()
      .then(setUser)
      .finally(() => setLoading(false));
  }, []);

  const value = useMemo(
    () => ({ user, loading, setUser }),
    [user, loading]
  );

  return (
    <AuthContext.Provider value={value}>
      {children}
    </AuthContext.Provider>
  );
}
```

Again, backend authorization is still required.

---

## Q157. Why can a context provider cause many renders?

Context consumers re-render when the provider's context value changes identity.

Bad:

```jsx
<AuthContext.Provider value={{ user, logout }}>
```

The object is newly created on every provider render.

Potentially better:

```jsx
const value = useMemo(
  () => ({ user, logout }),
  [user, logout]
);
```

But even a memoized context object doesn't make every context consumer selective by default. For large high-frequency contexts, split contexts or use a more targeted state subscription approach.

---

## Q158. How does memoization become slower and use more memory?

Memoization stores a value and checks dependencies to decide whether to reuse it.

If:

```text
computation cost < memoization overhead
```

then memoization can be a net loss.

Also, cached values can retain object graphs longer than a non-cached calculation would.

### Senior answer

> "Memoization is an optimization technique, not a correctness mechanism. I add it where profiling shows repeated expensive work or unstable identity is actually causing downstream cost."

---

## Q159. What is view recycling?

View recycling reuses rendered view instances for different data rather than continually creating and destroying new views.

Example:

```text
visible rows = 30

row view #1 displays record 500
scroll
row view #1 now displays record 530
```

This reduces allocation and creation churn.

Contrast with ordinary windowing, where items outside the visible window are removed and new ones are mounted.

---

## Q160. Can React recycle DOM nodes automatically?

Don't state that React's normal list rendering is equivalent to native RecyclerView-style recycling.

React reconciliation preserves and updates matching elements based on identity and keys, but standard React web rendering does not automatically implement full list view recycling for huge collections.

Virtualization libraries solve the large-list DOM problem explicitly.

---

# 24. Managerial Round — Conflict, Trade-offs, Communication

## Q161. How do you decide between SSE and WebSockets?

Ask:

```text
Does client need to send realtime messages?
Does server need to push updates?
How complex is reconnection?
What transport constraints exist?
```

Then:

```text
Server → client only → SSE
Bidirectional realtime → WebSocket
```

---

## Q162. How do you choose between CSR, SSR and SSG in a real project?

```text
SEO-sensitive + dynamic → SSR/dynamic
Mostly static + public  → SSG/pre-render
Highly interactive/private → CSR/client-heavy
```

Then layer caching/revalidation based on freshness requirements.

---

## Q163. How do you decide if a BFF is needed?

Use a BFF when:

- client must aggregate many backend services
- backend APIs aren't shaped for UI use
- security requires hiding internal topology
- frontend-specific caching/transformation is valuable
- mobile/web clients have different data needs

Avoid it when it adds a proxy layer without meaningful value.

---

# 25. Final Senior-Level Answering Framework

For almost every question in this guide, use this sequence:

```text
1. Define the concept
        ↓
2. Explain why it exists
        ↓
3. Explain internal behavior
        ↓
4. Give a real scenario
        ↓
5. Choose a solution
        ↓
6. Explain trade-offs
        ↓
7. Mention how you would measure/validate it
```

### Example: "How would you optimize a 10k-row React table?"

Weak:

> "Use React.memo and useMemo."

Strong:

> "First I'd profile whether the bottleneck is rendering, DOM size or data processing. If all 10k rows are mounted, virtualization is likely more important than memoization because it reduces DOM size. I'd combine that with server-side pagination if the product doesn't require all data locally, memoize expensive derived data only where it matters, and keep row props/selectors stable. Then I'd re-measure with the React Profiler and Chrome Performance panel."

### Example: "Postman works but browser fails."

Weak:

> "It's a CORS problem."

Strong:

> "The browser is enforcing its cross-origin policy. I would inspect the Network panel, determine whether an OPTIONS preflight occurs, verify the requested method/headers/credentials, and confirm that the server returns the correct CORS response headers. The frontend cannot bypass browser CORS enforcement."

### Example: "Why did you use TanStack Query instead of Redux?"

Strong:

> "Because the data was server state rather than client-owned workflow state. I wanted caching, deduplication, stale/fresh management, background refetching and mutation handling without manually rebuilding those concerns in Redux."

---

# 26. Rapid-Fire One-Liners

These are useful for the first 30 seconds of an answer.

- **Closure:** A function retains access to its lexical environment.
- **Event loop:** Coordinates synchronous JS execution with queued asynchronous callbacks/continuations.
- **Microtask:** High-priority queued continuation such as a Promise callback.
- **`===`:** Strict equality without the coercion performed by `==`.
- **Spread:** Expands; **Rest:** collects.
- **Shallow copy:** Copies the outer object but preserves nested references.
- **`??`:** Falls back only for null/undefined.
- **WeakMap:** Weakly held object-keyed associations that don't prevent eligible keys from being collected.
- **Fiber:** React's internal architecture for representing/scheduling rendering work.
- **Reconciliation:** React determines how the next UI tree differs from the previous one.
- **Virtualization:** Render only the visible window of a large collection.
- **View recycling:** Reuse existing rendered views for new data.
- **`useState`:** State that participates in rendering.
- **`useRef`:** Persistent mutable container that doesn't itself trigger a render.
- **`useMemo`:** Cache a calculated value when there is a real performance benefit.
- **`useCallback`:** Cache a function identity when that identity matters.
- **`React.memo`:** Skip a component render when its memo comparison says props are unchanged.
- **SSR:** Render on the server at request/dynamic-render time.
- **SSG:** Generate static output ahead of time.
- **CSR:** Render/complete UI primarily on the client.
- **Hydration:** Attach React behavior to server-generated HTML.
- **SSE:** Server → client event stream over HTTP.
- **WebSocket:** Bidirectional persistent communication channel.
- **BFF:** Backend service shaped for a particular frontend.
- **Tree shaking:** Static module analysis + dead-code elimination.
- **WCAG:** W3C accessibility guidelines for web content.
- **LCP:** Largest Contentful Paint.
- **INP:** Interaction to Next Paint.
- **CLS:** Cumulative Layout Shift.
- **XSS:** Attacker-controlled script/markup executes in a user's browser context.
- **CORS:** Browser-enforced cross-origin resource policy based on server-declared permissions.
- **401:** Authentication failure/missing credentials.
- **403:** Authenticated/understood but not authorized.

---

# 27. Official References for Current / Version-Sensitive Topics

- React Versions: https://react.dev/versions
- React 19: https://react.dev/blog/2024/12/05/react-19
- React 19.3: https://react.dev/blog/2026/09/09/react-19-3
- Next.js App Router: https://nextjs.org/docs/app
- Next.js Server and Client Components: https://nextjs.org/docs/app/getting-started/server-and-client-components
- Next.js Environment Variables: https://nextjs.org/docs/pages/guides/environment-variables
- Vite Features: https://vite.dev/guide/features
- Vite Dependency Pre-Bundling: https://vite.dev/guide/dep-pre-bundling
- WCAG 2.2: https://www.w3.org/TR/WCAG22/
- GitHub Actions: https://docs.github.com/en/actions/get-started/understanding-github-actions

---

# Final Revision Checklist

Before a senior frontend interview, be able to explain these without notes:

```text
Event Loop → Microtasks → Macrotasks/Tasks
Closure → Stale Closure
Reference equality → Shallow copy
React render → Reconciliation → Commit
Fiber → Concurrent rendering
useEffect → useLayoutEffect
useState → useReducer → useRef
React.memo → useMemo → useCallback
Keys → Identity
Virtualization → View recycling
CSR → SSR → SSG → Hydration
Redux → RTK → Saga → Context → TanStack Query
Optimistic updates → rollback
Caching → retries → cancellation
SSE → WebSocket
BFF → API contracts
Tree shaking → code splitting
Browser pipeline → layout → paint → composite
LCP → INP → CLS
WCAG → keyboard → focus → semantics
XSS → CSRF → cookies → CORS
Testing → unit → integration → E2E
GitHub Actions → CI/CD
Frontend HLD → scalability → availability → observability
```

The goal is not to memorize every word. The goal is to be able to **reason from first principles, choose a design, explain trade-offs, and connect the decision to a real frontend problem.**

---

# 28. Explicit Answers for Additional Question Variants

## Q164. Explain `addEventListener()` and JavaScript event handling.

`addEventListener` registers a function to run when a specific event occurs.

```js
const button = document.querySelector("button");

function handleClick(event) {
  console.log(event.type);
}

button.addEventListener("click", handleClick);
```

Remove it with the same function reference:

```js
button.removeEventListener("click", handleClick);
```

### Important options

```js
button.addEventListener("click", handleClick, {
  capture: true,
  once: true,
  passive: true
});
```

- `capture`: run during capture phase.
- `once`: automatically remove after the first invocation.
- `passive`: promises the handler won't call `preventDefault()`, allowing browsers to optimize some input/scroll handling.

### Event object

Useful properties include:

```text
target
currentTarget
type
bubbles
defaultPrevented
```

### `target` vs `currentTarget`

```js
parent.addEventListener("click", event => {
  console.log(event.target);       // actual clicked element
  console.log(event.currentTarget); // element with this listener
});
```

### React connection

React normally lets you write:

```jsx
<button onClick={handleClick}>Save</button>
```

For DOM/event-listener APIs outside React's declarative event props, use an effect with cleanup:

```jsx
useEffect(() => {
  window.addEventListener("resize", handleResize);

  return () => {
    window.removeEventListener("resize", handleResize);
  };
}, [handleResize]);
```

Be careful about function identity and effect dependencies so you don't repeatedly add/remove listeners unnecessarily.

---

## Q165. Explain debouncing and throttling.

### Debouncing

Wait until events stop for a specified period before running the operation.

Good for:

- search autocomplete
- validation
- resize calculations

```js
function debounce(fn, delay) {
  let timer;

  return function (...args) {
    clearTimeout(timer);

    timer = setTimeout(() => {
      fn.apply(this, args);
    }, delay);
  };
}
```

### Timeline

```text
A  B  C  D       stop
|  |  |  |
└──┴──┴──┴─ wait ─→ execute once
```

### Throttling

Limit execution to at most once within a window.

Good for:

- scroll
- mouse movement
- continuous resize telemetry

Conceptually:

```text
Events:  A B C D E F G H
Calls:   A     D     G
```

### Interview answer

> "Debounce waits until the burst of activity settles; throttle allows execution at a controlled frequency. I use debounce for search inputs and throttle for high-frequency events such as scroll."

---

## Q166. Explain `useState` and `useEffect`.

### `useState`

Stores state that participates in rendering.

```jsx
const [count, setCount] = useState(0);
```

When you call:

```js
setCount(prev => prev + 1);
```

React schedules an update and eventually renders the component with the new state snapshot.

### `useEffect`

Synchronizes the component with an external system after commit.

Examples:

- network connections
- subscriptions
- timers
- browser APIs
- analytics

```jsx
useEffect(() => {
  const timer = setInterval(() => {
    console.log("tick");
  }, 1000);

  return () => clearInterval(timer);
}, []);
```

### Dependency array

```jsx
useEffect(() => {
  // runs after relevant commits
}, [userId]);
```

The dependency list expresses the reactive values the effect uses and whose changes should cause the effect to re-synchronize.

### Common mistake

Using an effect just to derive data:

```jsx
useEffect(() => {
  setFullName(first + " " + last);
}, [first, last]);
```

Often better:

```jsx
const fullName = `${first} ${last}`;
```

Don't create a state/effect cycle for values that can be derived during render.

---

## Q167. What is Context API and what are its use cases?

Context lets a component make a value available to descendants without explicitly passing it through every intermediate component.

```jsx
const ThemeContext = createContext(null);

function App() {
  return (
    <ThemeContext.Provider value="dark">
      <Dashboard />
    </ThemeContext.Provider>
  );
}

function Dashboard() {
  const theme = useContext(ThemeContext);
  return <div data-theme={theme}>...</div>;
}
```

### Good use cases

- theme
- locale
- authentication/session information
- dependency/configuration objects
- relatively low-frequency shared state

### Poor use case

Huge high-frequency global state where many consumers update constantly.

That can cause broad re-render propagation and make ownership unclear.

For complex application state, Redux Toolkit or another store may provide more targeted subscriptions and richer state tooling. For server state, TanStack Query/SWR is usually a more natural abstraction.

### Senior answer

> "I use Context primarily for shared concerns that naturally form a provider boundary. I don't treat Context as a replacement for every form of state management."

---

## Q168. Explain Lazy Loading vs Code Splitting.

### Code splitting

Break application code into independently loadable chunks.

```text
main.js
admin.js
reports.js
checkout.js
```

### Lazy loading

Delay loading a chunk until it is needed.

```jsx
const Reports = lazy(() => import("./Reports"));
```

```jsx
<Suspense fallback={<Spinner />}>
  <Reports />
</Suspense>
```

### Why it helps

Without it:

```text
User opens Home
 ↓
Download Home + Admin + Reports + Settings + Checkout
```

With route-level splitting:

```text
User opens Home
 ↓
Download Home

User opens Reports
 ↓
Download Reports chunk
```

This reduces initial JavaScript when the boundaries are chosen well.

### Trade-offs

Over-splitting can cause:

- too many network requests
- waterfalls
- more loading states
- worse interaction if a required chunk wasn't prefetched or loaded in time

### Senior answer

> "I use code splitting to create meaningful loading boundaries and lazy loading to delay infrequently used code. I avoid splitting every component because the network overhead and loading waterfalls can outweigh the benefit."

---

## Q169. Explain React authentication strategies.

Common choices include:

### Cookie-based session

```text
Login
 ↓
Server creates session
 ↓
Secure HttpOnly cookie
 ↓
Browser sends cookie
 ↓
Server authenticates
```

### Access + refresh token architecture

```text
Login
 ↓
Short-lived access credential
+
Longer-lived refresh mechanism
```

The exact storage and rotation approach depends on the application threat model.

### OAuth / social login

```text
App
 ↓
Identity provider
 ↓
Authorization code
 ↓
Backend/token exchange
 ↓
Application session
```

### Important distinction

Route guards are not the security boundary. The backend must validate the user's authentication and authorization on protected APIs.

---

# 29. Final Cross-Reference Map

To make revision faster, use this map when the interviewer phrases the same concept differently:

| Interview wording | Study section |
|---|---|
| Event loop / execution context / call stack | Core JavaScript Q9 + Q10 |
| Promise / async-await / async tasks | Core JavaScript Q13–Q15 |
| Stale closure | Core JavaScript Q7 + React Q39 |
| Spread vs deep copy | Core JavaScript Q16–Q17 |
| `==` vs `===` | Core JavaScript Q11 |
| WeakMap / WeakSet | Core JavaScript Q19 |
| Event delegation / addEventListener | Q20 + Q164 |
| Debounce / throttle | Q165 + Q47 |
| `useState` / `useEffect` | Q166 + React hooks sections |
| Context API | Q167 + Q51 |
| Reconciliation / diffing / keys | Q28 + Q40 |
| Fiber / concurrent rendering | Q29 + Q30 |
| Hydration | Q60–Q61 |
| Server Components | Q31–Q32 + Q62 |
| SSR / SSG / CSR | Q58–Q59 |
| Bundle optimization | Q76 |
| Vite / Webpack | Q75 |
| Tree shaking | Q77 |
| Virtualization / windowing | Q71 |
| View recycling | Q159 |
| `useMemo` / `useCallback` / memo | Q36 + Q158 |
| Redux / RTK / Saga | Q49–Q52 |
| Context vs Redux vs Query | Q51 |
| Optimistic UI | Q54 + Q57 |
| API caching/retries | Q55 + Q101 |
| SSE / WebSocket | Q104 + Q161 |
| BFF | Q102 + Q163 |
| Authentication / JWT / RBAC | Q91–Q98 + Q169 |
| XSS / CORS / CSRF | Q95–Q96 |
| WCAG / accessibility | Q79–Q87 |
| Testing | Q88–Q90 |
| GitHub Actions / CI/CD | Q111–Q113 |
| Web Vitals | Q78 |
| SEO | Q114–Q116 |
| Top-K / HashMap / coding | C2 + C4 |
| Promise polyfill | C8 |
| Async concurrency scheduler | C9 |
| React-like class components | C10 |
| Pinterest HLD | Q123 |
| Collaborative editor | Q124 |
| SPA rate limiter | Q125 |
| Infinite scrolling | Q126 |
| Redux-like store | Q127 |
| OAuth/social auth | Q128 |
| Notification system | Q129 |
| Managerial / STAR | Q130–Q140 |
| Architect-level frontend strategy | Q141–Q150 |

---

# 30. Interview Closing Checklist

Before the interview, practice saying each answer aloud in this format:

> **"First I would clarify the requirement. Then I'd identify the bottleneck or consistency/security constraint. Based on that, I'd choose the simplest architecture that satisfies the requirement. I'd explain the trade-offs, implement it with clear boundaries, and validate it with tests and production metrics."**

For coding problems, say your assumptions and complexity before writing code.

For system design, always cover:

```text
Requirements
Architecture
Data flow
State ownership
API contracts
Caching
Failure handling
Security
Performance
Scalability
Observability
Trade-offs
```

For behavioral questions, use:

```text
Situation
Task
Action
Result
Learning
```

For project questions, never just list technologies. Explain:

```text
Problem → Decision → Implementation → Trade-off → Outcome
```

