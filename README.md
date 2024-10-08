# ⚛️ The Atomic Blog

A simple, dynamic blog application built with React that allows users to add, search, and archive blog posts. This application uses context for state management and hooks to manage component states.

## 🚀 Features

- Add Posts: Users can add posts by providing a title and body.
- Search Posts: Filter the list of posts by typing in the search bar.
- Clear Posts: Clear all posts at once.
- Archive: Show and add posts from a large archive (generated using Faker.js).
- Dark Mode Toggle: Switch between light and dark modes.

---

## 🛠️ Technologies Used

- React: A JavaScript library for building user interfaces.
- Context API: For state management across components.
- Faker.js: For generating random posts for the archive.
- CSS Modules: For styling components in a modular way.

---

## 🌐 Usage

1.Install dependencies:
npm install
2.Run the app:
npm start
4.Open your browser and navigate to `http://localhost:3000`.

---

## 🚧 How It Works

### 1. Post Management with Context API

The app uses `PostProvider` to manage the state of posts, search queries, and actions like adding or clearing posts.

- `usePosts`: A custom hook that provides access to the context state, making it easy to interact with the posts state from any component.
- `onAddPost`: Adds a new post to the list.
- `onClearPosts`: Clears all existing posts.

### 2. Dark Mode Toggle

The dark mode is controlled using `isFakeDark`, which toggles a class on the `document.documentElement` element.

### 3. Archive

An archive of 10,000 randomly generated posts is available. Users can add any of these archived posts as new posts in the current session.
