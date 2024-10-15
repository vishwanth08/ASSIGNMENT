<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Employee Registration</title>
    <link rel="stylesheet" href="styles.css"> <!-- Optional: Link to CSS file -->
</head>
<body>
    <h1>Employee Registration Form</h1>
    <form action="/submit-employee" method="POST">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="designation">Designation:</label>
        <input type="text" id="designation" name="designation" required>

        <label for="department">Department:</label>
        <select id="department" name="department" required>
            <option value="">Select a department</option>
            <option value="HR">HR</option>
            <option value="IT">IT</option>
            <option value="Finance">Finance</option>
            <option value="Marketing">Marketing</option>
            <option value="Sales">Sales</option>
        </select>

        <label for="salary">Salary:</label>
        <input type="number" id="salary" name="salary" required min="0" step="0.01">

        <label for="address">Address:</label>
        <textarea id="address" name="address" rows="4" required></textarea>

        <button type="submit">Register Employee</button>
    </form>
</body>
</html>