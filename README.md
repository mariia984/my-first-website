body {
    background: linear-gradient(120deg, #fdfbfb 0%, #ebedee 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    animation: fadeIn 1s ease-in-out;
}

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}

.profile-card {
    background: white;
    padding: 30px;
    border-radius: 16px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    text-align: center;
    max-width: 320px;
    animation: slideUp 0.8s ease forwards;
    opacity: 0;
}

@keyframes slideUp {
    from { transform: translateY(30px); opacity: 0; }
    to { transform: translateY(0); opacity: 1; }
}

.avatar {
    width: 120px;
    height: 120px;
    object-fit: cover;
    border-radius: 50%;
    margin-bottom: 20px;
    border: 4px solid #e1306c;
    animation: pulse 2s infinite;
}

@keyframes pulse {
    0% { box-shadow: 0 0 0 0 rgba(225, 48, 108, 0.5); }
    70% { box-shadow: 0 0 0 20px rgba(225, 48, 108, 0); }
    100% { box-shadow: 0 0 0 0 rgba(225, 48, 108, 0); }
}

h1 {
    margin: 0;
    font-size: 24px;
    color: #333;
}

p {
    color: #666;
    margin: 10px 0;
}

a {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 20px;
    background-color: #e1306c;
    color: white;
    text-decoration: none;
    border-radius: 30px;
    transition: background 0.3s ease, transform 0.3s ease;
}

a:hover {
    background-color: #c72a5c;
    transform: scale(1.05);
}

/* 🔻 Адаптація для телефону */
@media (max-width: 480px) {
    .profile-card {
        padding: 20px;
        max-width: 90%;
        margin: 20px;
    }

    h1 {
        font-size: 20px;
    }

    .avatar {
        width: 100px;
        height: 100px;
    }

    a {
        padding: 8px 16px;
        font-size: 14px;
    }
}
