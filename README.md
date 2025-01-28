# Redflix

Redflix is a sleek and intuitive web application that allows users to search for movies and view trending titles. Built with modern technologies like React, Vite, and Appwrite, Redflix offers a seamless movie discovery experience. 

## Features

- **Movie Search:** Search for movies using the [TMDB API](https://www.themoviedb.org/documentation/api).
- **Trending Movies:** View trending movies based on search counts aggregated through the Appwrite backend.
- **Responsive Design:** Optimized for mobile, tablet, and desktop with Tailwind CSS.
- **Debounced Search:** Reduces unnecessary API calls while typing in the search bar.
- **Dynamic Trending Section:** Updates automatically as search counts are recorded.
- **Fast Loading:** Powered by Vite for a high-performance development and build process.

## Tech Stack

- **Frontend:** React, Vite
- **Styling:** Tailwind CSS
- **Backend:** Appwrite
- **API Integration:** TMDB API
- **Build Tools:** Node.js, Vite

## Installation

Follow these steps to set up the project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/gopalbondz72344/redflix.git
   ```

2. Navigate to the project directory:
   ```bash
   cd redflix
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Set up environment variables:
   Create a `.env` file in the root of your project and add the following:
   ```env
   VITE_TMDB_API_KEY=your_tmdb_api_key
   VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
   VITE_APPWRITE_ENDPOINT=your_appwrite_endpoint
   ```
   Replace `your_tmdb_api_key`, `your_appwrite_project_id`, and `your_appwrite_endpoint` with your actual credentials.

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Open your browser and navigate to:
   ```
   http://localhost:5173
   ```

## Deployment

To deploy the application, build the production version and serve it:

1. Build the app:
   ```bash
   npm run build
   ```

2. Serve the built files:
   ```bash
   npm run preview
   ```

You can also deploy Redflix to any static hosting service such as Netlify, Vercel, or AWS S3.

## API Usage

Redflix relies on the TMDB API for fetching movie data. Ensure you have an API key by creating an account on [TMDB](https://www.themoviedb.org/). Use the key in the `.env` file as shown above.

### Key Endpoints

- **Search Movies:**
  ```
  GET /search/movie?api_key=<API_KEY>&query=<MOVIE_NAME>
  ```
- **Trending Movies:**
  Handled via the Appwrite backend.

## Contributing

We welcome contributions to make Redflix even better! To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to your fork:
   ```bash
   git push origin feature-name
   ```
5. Create a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- [TMDB API](https://www.themoviedb.org/documentation/api) for movie data.
- [Appwrite](https://appwrite.io/) for backend support.
- [Tailwind CSS](https://tailwindcss.com/) for responsive design.

---

Happy streaming! 🎥🍿
