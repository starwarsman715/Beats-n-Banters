# Beats n Banters - Spotify Playlist Generator

This repository contains the final project for **CS 411**.  
**Beats n Banters** is a web application that generates Spotify playlists based on randomly generated quotes.  
Each word in a quote corresponds to a song that is added to the playlist, creating a unique and fun experience for the user.

## Technologies Used

### Frontend
- **Next.js**: React framework for modern web applications, used for the user interface and routing.
- **Ant Design**: UI component library for React, used to create forms and visually appealing elements.
- **TypeScript**: Statically typed language that improves code quality and maintainability.
- **CSS Modules**: For local and global styling.
- **REST API**: Communication with the backend and external services.

The frontend code is located in the [`client`](client/README.md) folder.  
Notable files include:
- Pages in [`client/pages`](client/pages/index.tsx)  
- Styles in [`client/styles`](client/styles/globals.css)  
- Configuration in [`client/next.config.js`](client/next.config.js)  

### Backend
- **Express.js**: Node.js framework that handles routing and server logic.
- **MongoDB**: NoSQL database used to store user information and authentication tokens.
- **Mongoose**: ODM for MongoDB that simplifies database interactions.
- **CORS**: Middleware to allow requests between frontend and backend.
- **Request**: Library to make HTTP requests to the Spotify API.
- **Spotify Web API**: Used to authenticate users, create playlists, and add songs.

The backend is organized in the [`server`](server/server.js) folder, with the main file being [`server/server.js`](server/server.js).

## Project Structure
- [`client`](client/README.md): Contains all frontend code, including pages, components, styles, and configuration.
- [`server`](server/server.js): Contains backend code, Spotify authentication logic, and database interaction.
- [`package.json`](package.json): Root file for general dependencies.
- [`CS411 Ideas.pdf`](CS411%20Ideas.pdf): Document containing project brainstorming and ideas.

## How It Works
1. The user enters their Spotify username and desired playlist title in the web interface.
2. Clicking "Create" starts the authentication process with Spotify.
3. Once authenticated, a random quote is generated using the Techy API.
4. For each word in the quote, a matching song is searched on Spotify and added to the new playlist.
5. The user is redirected and can view the generated playlist in their Spotify account.

## Useful Links
- [Demo Video](https://drive.google.com/file/d/10ZcAo1bhdb4bepdkU_n97LVaLUDqB9Lx/view)

## Authors
This project was carried out by:
- Raquel Gonzalez  
- Martin Herguedas  
- Brianna Li  
- Andre Weiss
