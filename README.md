# Netflix Clone

## Table of Contents
1. Prerequisites
2. Features
3. Third-Party Libraries Used
4. Installation with Docker
5. Todo

## Prerequisites
- Create an account on a movie database platform to get an API key.
- Follow the platform's documentation to generate an API key.
- If using version 3 of the API, create a `.env` file and copy the content of `.env.example`. Then, paste the API key.

## Features
- Custom Hooks implementation
- Context API usage with provider
- Code-Splitting using lazy and Suspense
- Lazy loading feature to reduce bundle size
- Data loading and Redux dispatch in loaders
- Portal usage for rendering components outside the DOM hierarchy
- Forwarding Refs for reusable components
- Higher-Order Components (HOC) for component reuse
- Customizing the default theme of Material UI
- Redux Toolkit and RTK Query for state management
- Customizing class names in Material UI
- Infinite Scrolling using Intersection Observer API
- Carousel implementation

## Third-Party Libraries Used
- React Router
- Material UI
- Framer Motion
- Video.js
- React Slick

## Installation with Docker
```sh
docker build --build-arg TMDB_V3_API_KEY=your_api_key_here -t netflix-clone .
docker run --name netflix-clone-website --rm -d -p 80:80 netflix-clone
```

## Todo
- Improve animation of video card portal
- Optimize performance to prevent unnecessary re-renders
- Replace bundler with a more efficient option when available
- Improve accessibility for better user experience
- Add tests for better reliability

