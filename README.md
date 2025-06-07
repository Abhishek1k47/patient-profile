<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Patient Profile</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
    }

    .profile-container {
      display: flex;
      height: 100vh;
      background: #f8f9fa;
    }

    .sidebar {
      width: 250px;
      background: white;
      padding: 20px;
      border-right: 1px solid #e0e0e0;
    }

    .sidebar .avatar {
      width: 100px;
      height: 100px;
      border-radius: 50%;
    }

    .sidebar h3 {
      margin-top: 15px;
      font-size: 20px;
    }

    .sidebar p {
      font-size: 14px;
      margin: 4px 0;
      color: #666;
    }

    .sidebar ul {
      padding: 0;
      list-style: none;
      margin-top: 20px;
    }

    .sidebar ul li {
      padding: 10px 0;
      font-size: 15px;
      color: #444;
      cursor: pointer;
    }

    .sidebar ul li a {
      text-decoration: none;
      color: inherit;
    }

    .sidebar ul li a:hover {
      color: #4b2aad;
      text-decoration: underline;
    }

    .active-btn {
      margin-top: 20px;
      padding: 10px;
      background: #4b2aad;
      color: white;
      border: none;
      width: 100%;
      border-radius: 8px;
      cursor: pointer;
    }

    .main-form {
      flex-grow: 1;
      padding: 40px;
      background: #f1f4f8;
    }

    .main-form h2 {
      margin-bottom: 20px;
    }

    .main-form form {
      max-width: 500px;
    }

    .main-form input,
    .main-form select {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 6px;
    }

    .main-form button {
      margin-top: 15px;
      background: #4b2aad;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div class="profile-container">
    <div class="sidebar">
      <img src="https://via.placeholder.com/100" class="avatar" />
      <h3>John Doe</h3>
      <p>Patient ID: 123456</p>
      <p>Male</p>
      <ul>
        <li><a href="https://zcform.com/XMeM0" target="_blank">My Appointments</a></li>
        <li>Favourites</li>
        <li>Help</li>
        <li>My Wallet</li>
        <li>Messages</li>
        <li>Notifications</li>
      </ul>
      <button class="active-btn">Profile Settings</button>
    </div>

    <div class="main-form">
      <h2>Profile Settings</h2>
      <form>
        <label>Upload Image</label><br>
        <input type="file" /><br><br>

        <input type="text" placeholder="Enter Name" />
        <input type="email" placeholder="Enter Email" />
        <select>
          <option>Male</option>
          <option>Female</option>
          <option>Other</option>
        </select>
        <input type="tel" placeholder="Mobile Number" />
        <input type="date" />
        <select>
          <option>India</option>
          <option>USA</option>
          <option>UK</option>
        </select>
        <button type="submit">Save</button>
      </form>
    </div>
  </div>
</body>
</html>
