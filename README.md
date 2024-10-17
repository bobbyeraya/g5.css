g5.css
body {
    background: #f4f4f4;
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    overflow-x: hidden;
}body {
    background-image: url('pics/bg2.png');
    background-size: cover; /* Adjusts the background image to cover the entire page */
    background-position: center; /* Centers the background image */
    background-repeat: no-repeat; /* Ensures the background image does not repeat */
}

header {
    background: #667a6a;
    color: #fff;
    padding: 20px;
    text-align: center;
}

main {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 20px;
}

.team-member {
    background: #d6cdcd;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    margin: 10px;
    padding: 15px;
    width: 300px;
    text-align: center;
    cursor: pointer;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.team-member:hover {
    transform: translateY(-10px);
    box-shadow: 0 6px 12px rgba(0,0,0,0.3);
}

.team-member img {
    width: 100%;
    border-radius: 50%;
    transition: transform 0.3s ease;
}

.team-member img:hover {
    transform: scale(1.1);
}

.team-member h2 {
    margin: 15px 0;
    font-size: 1.5em;
    color: #333;
}

.team-member p {
    color: #666;
}

.team-member a {
    display: inline-block;
    margin: 5px 10px;
    color: #007BFF;
    text-decoration: none;
    font-size: 1em;
    text-align: center;
}

.team-member a:hover {
    text-decoration: underline;
}

footer {
    color: #131212;
    padding: 10px;
    text-align: center;
    position: relative;
    bottom: -170px;
    width: 100%;
}

.modal {
    display: none;
    position: fixed;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.5);
    justify-content: center;
    align-items: center;
    z-index: 1000;
    transition: opacity 0.3s ease;
}

.modal-content {
    background: #fff;
    padding: 20px;
    border-radius: 8px;
    width: 80%;
    max-width: 600px;
    position: relative;
    animation: slideIn 0.3s ease-out;
}

.modal-content img {
    width: 100%;
    border-radius: 8px;
    transition: transform 0.3s ease;
}

.modal-content h2 {
    margin-top: 15px;
    color: #333;
}

.modal-content p {
    color: #666;
}

.modal .close-btn {
    position: absolute;
    top: 10px;
    right: 10px;
    font-size: 24px;
    color: #333;
    background: #f4f4f4;
    border: none;
    cursor: pointer;
    transition: color 0.3s ease;
}

.modal .close-btn:hover {
    color: #007BFF;
}
.social-buttons {
    margin-top: 15px;
    text-align: center;
}

.social-button {
    display: inline-block;
    margin: 5px;
    padding: 10px 20px;
    color: #fff;
    background-color: #007BFF;
    text-decoration: none;
    border-radius: 5px;
    font-size: 1em;
    transition: background-color 0.3s ease;
}

.social-button:hover {
    background-color: #0056b3;
    text-align: center;
}

@keyframes slideIn {
    from {
        transform: translateY(-50px);
        opacity: 0;
    }
    to {
        transform: translateY(0);
        opacity: 1;
    }
}
