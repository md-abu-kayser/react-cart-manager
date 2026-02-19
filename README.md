# React Cart Manager - LocalStorage & Data-Driven UI

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
- **GitHub:** [github.com/abu.kayser-official](https://github.com/md-abu-kayser)
- **Email:** [abu.kayser.official@gmail.com](mailto:abu.kayser.official@gmail.com)

If you’d like this README tailored for a specific purpose - such as **hiring managers**, **open-source contributors**, or **client deliverables** - feel free to request a custom tone or format.

---

It’s designed to be **clean, well-structured**, and **pleasant to explore** - perfect for practice.
**Thank you for reviewing this project!**

---
