Author: Aaryaman Jaising

# 🎬 MovieFinder

A sleek and intuitive movie discovery app built with **React + Vite**, styled with **Tailwind CSS**, and powered by the **TMDB API** and **Appwrite**. The app allows users to search for movies, explore trending titles, and get simple recommendations—all within a fast, modern UI.

![App Screenshot](./public/screenshot.png) <!-- Replace with actual image path or URL -->

---

## 🚀 Live Demo

👉 [Live App](https://your-vercel-url.vercel.app)  
📁 [GitHub Repo](https://github.com/Ar4yu/movie-app)

---

## 🎓 Based On

This project was inspired by and partially based on a tutorial by **JavaScript Mastery**:

📺 [Build and Deploy a React Movie App | JavaScript Mastery (YouTube)](https://www.youtube.com/watch?v=dCLhUialKPQ)

> I followed this tutorial as a learning resource and built upon it with my own features, styling, and deployment setup.

---

## 🧠 Project Overview

The app fetches movie data from the [TMDB API](https://www.themoviedb.org/documentation/api) and allows users to:

- 🔍 Search for movies by title
- 🌟 View trending/popular movies
- 💡 Get movie card details (poster, rating, summary, etc.)
- 📈 Track searched movies via Appwrite (optional backend)

### 📈 Simple Trending Algorithm

The **trending movies** section pulls data from a backend (Appwrite), which tracks how often a movie appears in a user’s search. The process is:

1. A user searches for a movie.
2. If a valid result is returned, the app records the **first result**.
3. These are stored with a **search count** per movie ID.
4. The app then sorts the list by **highest search count**, creating a basic but effective popularity tracker.

> This logic is handled in the backend using Appwrite’s database, making it simple but extendable for future personalization.

---

## ✨ Features

- 🔍 Real-time debounced search
- 🎯 TMDB-powered discover and search APIs
- 🧾 Appwrite backend logging (basic recommendation engine)
- ⚡ Fast development with Vite and React
- 📱 Responsive layout using Tailwind CSS

---

## 🧰 Tech Stack

| Tool         | Purpose                              |
| ------------ | ------------------------------------ |
| React        | Frontend framework                   |
| Vite         | Build tool for fast dev              |
| Tailwind CSS | Utility-first styling                |
| TMDB API     | Movie data (titles, images, etc.)    |
| Appwrite     | Optional backend (logging & storage) |

---

## 🛠️ Environment Variables

```env
VITE_TMDB_API_KEY=your_tmdb_v3_api_key
VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
VITE_APPWRITE_DATABASE_ID=your_appwrite_db_id
VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
```
