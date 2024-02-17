# Chat Room

### Live Chat Application using Python, Flask & SocketIO 

This project implements a real-time chat web app with multiple rooms, using Python, Flask, and SocketIO.

## Overview

The app allows users to join chat rooms and communicate with others in real-time. New users can easily create a username and jump into available chat rooms. 

Rooms are topic-based for focused discussions. The interface shows who is online in each room as well as a history of messages. Behind the scenes, SocketIO enables bidirectional communication for instant messaging between clients and the server.

## Key Features

- **Multiple chat rooms** for different topics and interests
- **Real-time messaging** with smooth user experience
- **User list** to see who is online in each room  
- **Message history** to view past conversations 
- **Simple username** creation for getting started quickly
- **Responsive design** for optimal viewing on any device

## How It Works

The Flask server manages chat rooms and users. When a new user connects, they are assigned a random room by default. The username is stored along with the active room.

SocketIO events handle messaging between clients and the server. The 'message' event queues new messages which are then broadcast to others in the same room. A history of messages is also maintained. 

The front-end uses JavaScript and jQuery to listen for SocketIO events and update the UI. Users can seamlessly send messages, change rooms, and view past discussions.

## Running the App

The app requires Python 3 and the following packages:

- Flask
- Flask-SocketIO

To start:

1. Install requirements
2. Run `python app.py`
3. Navigate to `http://localhost:5000`

The main app logic is contained in `app.py`. Static assets are served from the `static` folder.

## Next Steps

Future improvements for this project:

- Private messaging between users
- User authentication 
- Custom room creation
- Support for images, links, videos
- Mobile optimizations
- UI enhancements
