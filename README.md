'DummyChatApp' is a realtime Web-Chat application which allows multiple users to communicate and coordinate with each other via different mediums effectively. 

## Setup 

Clone the Git Repository

`https://github.com/urffsamhunt/chat`

then

```bash
cd chat
npm install
```

To run the development server:
```bash
npm run dev
```
To run the release build:
```bash
npm build
npm run start
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

Note that you will also need to set up the `.env.local` file in the root of the project directory and set the following parameters accordingly (Supabase):

```env
NEXT_PUBLIC_SUPABASE_URL
NEXT_PUBLIC_SUPABASE_ANON_KEY
```

## Automatic Setup along with Supabase and Vercel (TODO)


### Feature Roadmap
    [x] Project Setup
        [x] Initialize repository with proper structure
        [x] Set up development environment
    [x] User Authentication
        [x] Registration and login system
        [x] User profiles with customizable avatars
        [x] Session management
        [x] Password recovery mechanism
    [x] Basic Chat Interface
        [x] Clean, responsive UI
        [x] Message input and display
        [x] Basic conversation threading
        [x] Read receipts along with timestamp
    [ ] Real-time Communication
        [x] Implement websocket connections
        [x] Message delivery status indicators
        [x] Typing indicators
        [ ] Online/offline status
    [ ] Advanced Chat Features
        [ ] Group chat functionality
        [x] Direct messaging between users
        [ ] Message reactions (likes, emoji responses)
    [ ] Media Support
        [ ] Image sharing and previews
        [ ] File attachments
        [ ] Link previews
        [ ] Voice messages (optional)

Day 3: Polish & Other Optional Features

    [ ] Search & Organization
        [ ] Message search functionality
        [ ] Chat history
        [ ] Message threading/replies
        [ ] Pin important messages
    [ ] Notifications
        [ ] Real-time notifications
        [ ] Email notifications (optional)
        [ ] Notification preferences
        [ ] Mention functionality (@username)
    [ ] Final Touches
        [ ] Theme customization (light/dark mode)
        [ ] Performance optimization

## Code Structure

- src
    - app
        - api (Contains all API endpoints)
        - auth (Authentication Confirmation related utilities)
        - authentication (Login / Sign Up Page)
        - utils (Utilities related to Supabase Clients)
        - chat (Main Chat Interface)
