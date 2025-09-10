body {
  font-family: Arial, sans-serif;
  background: #f9fafb;
  margin: 0;
  padding: 0;
}

.app {
  max-width: 900px;
  margin: 20px auto;
  padding: 20px;
}

.header {
  text-align: center;
}

.subtitle {
  color: #666;
}

.dark {
  background: #1a1a1a;
  color: white;
}

.dark .book-card {
  background: #333;
}

.search {
  display: flex;
  gap: 10px;
  margin: 20px 0;
}

.search input {
  flex: 1;
  padding: 10px;
  font-size: 1rem;
}

.search button {
  padding: 10px 15px;
  background: #2563eb;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.results {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 15px;
}

.book-card {
  background: white;
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 10px;
  text-align: center;
}

.book-card img {
  max-width: 100%;
  border-radius: 5px;
}

.no-cover {
  background: #eee;
  padding: 20px;
  border-radius: 5px;
}

.more-info-btn,
.fav-btn {
  display: block;
  margin: 10px auto 0;
  padding: 8px 12px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.more-info-btn {
  background: #10b981;
  color: white;
}

.fav-btn {
  background: #f43f5e;
  color: white;
}

.pagination {
  margin: 20px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.favorites {
  margin-top: 40px;
}

.spinner-container {
  text-align: center;
}

.spinner {
  border: 4px solid #f3f3f3;
  border-top: 4px solid #2563eb;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  animation: spin 1s linear infinite;
  margin: 0 auto;
}

@keyframes spin {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

.error {
  color: red;
  text-align: center;
}
.clear-btn {
  padding: 10px 15px;
  background: #6b7280;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.clear-btn:hover {
  background: #4b5563;
}
.sorting {
  margin: 15px 0;
  text-align: center;
}

.sorting select {
  padding: 8px;
  border-radius: 5px;
  font-size: 1rem;
}
.fav-btn {
  margin-top: 10px;
  padding: 8px 12px;
  border: none;
  background: #e5e7eb;
  border-radius: 5px;
  cursor: pointer;
}

.fav-btn.active {
  background: gold;
  font-weight: bold;
}

.favorites {
  margin: 30px 0;
  padding: 20px;
  background: #f9fafb;
  border-radius: 10px;
}

.favorites h2 {
  margin-bottom: 15px;
}

.favorites-list {
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
}

.fav-card {
  background: white;
  padding: 10px;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}
/* 📱 Responsive Design */
@media (max-width: 768px) {
  .results {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 15px;
  }

  .book-card {
    font-size: 0.9rem;
    padding: 10px;
  }

  .book-card img {
    height: 150px;
  }

  .favorites-list {
    flex-direction: column;
  }
}

@media (max-width: 480px) {
  .results {
    grid-template-columns: 1fr;
  }

  .book-card {
    font-size: 0.85rem;
    text-align: center;
  }

  .book-card img {
    height: 140px;
  }
}
/* 🔄 Spinner Styles */
.spinner-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 20px 0;
}

.spinner {
  border: 4px solid #f3f3f3; /* Light gray */
  border-top: 4px solid #2563eb; /* Blue */
  border-radius: 50%;
  width: 40px;
  height: 40px;
  animation: spin 1s linear infinite;
}

@keyframes spin {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
.clear-btn {
  background: #ef4444; /* red */
  color: white;
  border: none;
  padding: 10px 15px;
  border-radius: 6px;
  cursor: pointer;
  font-weight: 600;
}

.clear-btn:hover {
  background: #dc2626;
}
.results-info {
  margin: 10px 0;
  font-size: 0.95rem;
  color: #374151;
  text-align: center;
}
.pagination {
  margin-top: 20px;
  display: flex;
  justify-content: center;
  gap: 15px;
  font-size: 1rem;
}

.pagination button {
  padding: 8px 14px;
  border: none;
  background: #2563eb;
  color: white;
  border-radius: 5px;
  cursor: pointer;
}

.pagination button:disabled {
  background: #9ca3af;
  cursor: not-allowed;
}
