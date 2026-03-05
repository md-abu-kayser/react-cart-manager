# React Cart Manager - LocalStorage & Data-Driven UI

<!-- MIT License -->

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

<!-- CSS -->

[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)

<!-- Languages & Web Standards -->

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![ECMAScript Spec](https://img.shields.io/badge/ECMAScript-262-7A0BC0?logo=ecmascript&logoColor=white)](https://www.ecma-international.org/publications-and-standards/standards/ecma-262/)

<!-- Infra & Runtime -->

[![Node.js](https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)

<!-- Testing -->

[![Jest](https://img.shields.io/badge/Jest-C21325?logo=jest&logoColor=white)](https://jestjs.io/)

## Plain docs links
- CSS (MDN) docs: [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- JavaScript (MDN) docs: [https://developer.mozilla.org/en-US/docs/Web/JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- ECMAScript (spec, ECMA-262) docs: [https://www.ecma-international.org/publications-and-standards/standards/ecma-262/](https://www.ecma-international.org/publications-and-standards/standards/ecma-262/)
- Node.js docs: [https://nodejs.org/](https://nodejs.org/)
- React docs: [https://react.dev/](https://react.dev/)
- Jest docs: [https://jestjs.io/](https://jestjs.io/)

---

A small, well-structured React demo app that demonstrates component composition, simple client-side data fetching, and localStorage-based cart utilities. It was bootstrapped with Create React App and is intended as a polished portfolio piece.

## Highlights

- Clean component layout and CSS modules for scoped styling.
- Simple utilities for arithmetic and localStorage-based cart management.
- Data-driven UI using a local JSON file ([public/data.json](public/data.json)).
- Ready-to-run with standard CRA scripts.

## Quick start

1. Install
   ```sh
   npm install
   ```
2. Run locally

```sh
   npm start

```

3. Run tests

```sh
npm test
```

4. Build for production

```sh
   npm run build
```

## What to look at (key files and symbols)

1. **Root and entry**

- App component: App - src/App.js
- React entry: src/index.js

2. **Components**

- Cosmetics list: Cosmetics - src/components/Cosmetics/Cosmetics.js
- Cosmetic item: Cosmetic - src/components/Cosmetic/Cosmetic.js
- Shoes demo: Shoes - src/components/Shoes/Shoes.js
- Cloath demo: Cloath - src/components/Cloath/Cloath.js

3. **Utilities**

- Arithmetic helpers: add, multiply, divided, getTotal - src/components/utilites/calculetor.js
- Local storage cart helpers: addToDb, removeFromDb, deleteShoppingCart - src/components/utilites/fakedb.js

4. **Styles**

- Global: src/index.css
- App: src/App.css
- Cosmetic item: src/components/Cosmetic/Cosmetic.css

5. **Tests and tooling**

- Tests setup: src/setupTests.js
- Performance helper: src/reportWebVitals.js

6. **Bundled and public assets**

- Local JSON used by the demo: public/data.json and build output build/data.json
- Package metadata: package.json
- Git ignore: .gitignore

  **Design notes - what to mention to a client**

- The UI is data-driven:- the Cosmetics component fetches public/data.json and renders Cosmetic items.
- Cart persistence is implemented with a minimal API in fakedb that stores a JSON map in localStorage; the functions addToDb and removeFromDb are intentionally small and easy to extend or replace with a remote API.
- Utilities in calculetor show simple pure functions (add, multiply, divided, getTotal) that are easy to unit-test and reuse across components.

7. **Example usage**

**Import utilities:**

```
  import { add, multiply } from './components/utilites/calculetor';

```

**Using cart helper in a component:**

```
  import { addToDb } from './components/utilites/fakedb';
```

addToDb(productId);

### Contributing

- Small, focused PRs are welcome. Follow the existing code style and keep components single-responsibility.
- Use the existing utility functions or add new pure helpers under src/components/utilites.

### License

- This project is licensed under the terms of the **[MIT License](./LICENSE)**.
- You may replace or update the license as needed for client or proprietary projects.

---

### Contact and Maintainer

- **Project:** _react-cart-manager_
- **Name:** Md Abu Kayser - Full-Stack Engineer
- **Maintainer:** [md-abu-kayser](https://github.com/md-abu-kayser)
- **Email:** [abu.kayser.official@gmail.com](mailto:abu.kayser.official@gmail.com)
- **GitHub:** [github.com/abu.kayser-official](https://github.com/md-abu-kayser)

If you’d like this README tailored for a specific purpose - such as **hiring managers**, **open-source contributors**, or **client deliverables** - feel free to request a custom tone or format.

---

It’s designed to be **clean, well-structured**, and **pleasant to explore** - perfect for practice.
**Thank you for reviewing this project!**

---
