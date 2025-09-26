# Movie Search Application

A modern React application for discovering and searching movies using The Movie Database (TMDb) API. Built with Vite, Tailwind CSS, and modern React hooks.

<img width="1470" height="825" alt="image" src="https://github.com/user-attachments/assets/b7fa8b7f-e0f0-4765-aa2d-f148d948d470" />
<img width="1470" height="829" alt="image" src="https://github.com/user-attachments/assets/0462004c-d0d5-4d4c-b957-43edee91de34" />
<img width="1470" height="823" alt="image" src="https://github.com/user-attachments/assets/59fa7669-30e1-4973-995d-d0354f25e862" />




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
- **Appwrite** - Backend as a Service for database
- **react-use** - Collection of React hooks
- **JavaScript (ES6+)** - Programming language

## Prerequisites

Before running this application, make sure you have:

- Node.js (version 16 or higher)
- npm or yarn package manager
- TMDb API key (free registration at https://www.themoviedb.org/settings/api)
- Appwrite account and project (free at https://appwrite.io/)

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

4. Add your API keys and configuration to `.env`:
```
VITE_TMDB_API_KEY=your_tmdb_api_key_here
VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
VITE_APPWRITE_PROJECT_NAME=your_project_name
VITE_APPWRITE_ENDPOINT=https://fra.cloud.appwrite.io/v1
VITE_APPWRITE_DATABASE_ID=your_database_id
VITE_APPWRITE_COLLECTION_ID=metrics
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
| `VITE_APPWRITE_PROJECT_ID` | Appwrite project ID | Yes |
| `VITE_APPWRITE_PROJECT_NAME` | Appwrite project name | Yes |
| `VITE_APPWRITE_ENDPOINT` | Appwrite endpoint URL | Yes |
| `VITE_APPWRITE_DATABASE_ID` | Appwrite database ID | Yes |
| `VITE_APPWRITE_COLLECTION_ID` | Appwrite collection ID for metrics | Yes |

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [The Movie Database (TMDb)](https://www.themoviedb.org/) for providing the movie data API
- [Tailwind CSS](https://tailwindcss.com/) for the styling framework
- [Vite](https://vitejs.dev/) for the fast build tool




