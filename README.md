# Job Portal 🚀

A full-stack job portal application where users can browse jobs, apply, companies can post jobs, and admins can manage everything.

## ✨ Features

- **Job Browsing & Search**: Filter jobs by category, latest jobs carousel
- **User Authentication**: Login/Signup with JWT
- **User Profiles**: Update profile, view applied jobs
- **Company Features**: Company profiles, post jobs
- **Job Applications**: Apply to jobs, track applications
- **Admin Dashboard**: Manage jobs, companies, applicants
- **Responsive UI**: Modern design with Tailwind CSS & shadcn/ui

## 🛠️ Tech Stack

| Frontend          | Backend         | Database | Others        |
| ----------------- | --------------- | -------- | ------------- |
| React 18          | Node.js/Express | MongoDB  | Redux Toolkit |
| Vite              | Mongoose ODM    |          | JWT Auth      |
| Tailwind CSS      | Multer          |          | Cloudinary    |
| Radix UI / shadcn | bcryptjs        |          | Axios         |
| React Router      | Nodemon         |          |               |

## 📋 Prerequisites

- Node.js (v18+)
- MongoDB (local or Atlas)
- Cloudinary account (for media uploads)
- npm or yarn

## 🚀 Quick Start

### Backend Setup

1. Navigate to backend:

   ```bash
   cd backend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create `.env` file (see Environment Variables below)

4. Start server:
   ```bash
   npm run dev
   ```
   Server runs on `http://localhost:5000`

### Frontend Setup

1. Navigate to frontend:

   ```bash
   cd frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start dev server:
   ```bash
   npm run dev
   ```
   App runs on `http://localhost:5173`

## 🔧 Environment Variables

### Backend `.env`

```
NODE_ENV=development
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

### Frontend `.env` (optional)

```
VITE_API_URL=http://localhost:5000/api
```

## 📁 Folder Structure

```
jobportal/
├── backend/
│   ├── controllers/     # API logic
│   ├── models/          # Mongoose schemas
│   ├── routes/          # Express routes
│   ├── middlewares/     # Auth, upload middleware
│   └── utils/           # DB, Cloudinary helpers
├── frontend/
│   ├── src/
│   │   ├── components/  # UI components (auth, jobs, admin)
│   │   ├── hooks/       # Custom React hooks
│   │   ├── redux/       # Redux slices & store
│   │   └── utils/       # Constants, helpers
│   └── public/
└── README.md
```

## 🌐 API Endpoints (Base: `/api`)

- **Auth**: `POST /user/register`, `POST /user/login`
- **Jobs**: `GET /job`, `POST /job` (admin), `GET /job/:id`
- **Companies**: `GET /company`, `POST /company` (admin)
- **Applications**: `POST /application/apply/:jobId`, `GET /application/my`

## 🧪 Testing

Backend has no tests configured. Add with `npm test`.

## 🤝 Contributing

1. Fork the repo
2. Create branch: `git checkout -b feature-name`
3. Commit: `git commit -m 'Add feature'`
4. Push: `git push origin feature-name`
5. Open PR

## 📸 Screenshots

<img width="1890" height="866" alt="image" src="https://github.com/user-attachments/assets/0c454110-bfd0-42db-99e5-ede2a9e9a15e" />

<img width="1862" height="802" alt="image" src="https://github.com/user-attachments/assets/fc512c3e-5b81-410d-bf79-a7e0f095b091" />


## 📄 License

This project is open-source under ISC License.
