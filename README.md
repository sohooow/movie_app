# Movie Search Application

A modern React application for discovering and searching movies using The Movie Database (TMDb) API. Built with Vite, Tailwind CSS, and modern React hooks.

## Features

- Search movies by title
- Browse trending and popular movies
- Debounced search to optimize API requests
- Responsive design with Tailwind CSS
- Movie details display with posters
- Loading states and error handling

## Technologies Used

- **React 19** - Frontend library
- **Vite** - Build tool and development server
- **Tailwind CSS** - Utility-first CSS framework
- **TMDb API** - Movie data source
- **react-use** - Collection of React hooks
- **JavaScript (ES6+)** - Programming language

## Prerequisites

Before running this application, make sure you have:

- Node.js (version 16 or higher)
- npm or yarn package manager
- TMDb API key (free registration at https://www.themoviedb.org/settings/api)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/sohooow/movie_app.git
cd movie_app
```

2. Install dependencies:
```bash
npm install
```

3. Create environment file:
```bash
cp .env.example .env
```

4. Add your TMDb API key to `.env`:
```
VITE_TMDB_API_KEY=your_api_key_here
```

## Usage

### Development

Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5173/`

## Project Structure

```
src/
├── components/          # Reusable React components
│   ├── Search.jsx      # Search input component
│   ├── MovieCard.jsx   # Movie display component
│   └── Spinner.jsx     # Loading indicator
├── App.jsx             # Main application component
├── main.jsx           # Application entry point
└── index.css          # Global styles and Tailwind imports
```

## API Integration

This application uses The Movie Database (TMDb) API to fetch movie data. The following endpoints are utilized:

- `/discover/movie` - Popular movies
- `/search/movie` - Search movies by query

## Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `VITE_TMDB_API_KEY` | Your TMDb API key | Yes |

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [The Movie Database (TMDb)](https://www.themoviedb.org/) for providing the movie data API
- [Tailwind CSS](https://tailwindcss.com/) for the styling framework
- [Vite](https://vitejs.dev/) for the fast build tool




