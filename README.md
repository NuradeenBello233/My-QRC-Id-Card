<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Identity Card Form</title>
    <style>
        body { font-family: Arial, sans-serif; max-width: 600px; margin: auto; padding: 20px; }
        label { display: block; margin-top: 10px; }
        input, select { width: 100%; padding: 8px; margin-top: 5px; }
        .upload-area { margin-top: 10px; }
        button { margin-top: 20px; padding: 10px 15px; }
    </style>
</head>
<body>

<h2>Identity Card Details</h2>
<form action="/submit-id-card" method="POST" enctype="multipart/form-data">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="staff_number">Staff Number:</label>
    <input type="text" id="staff_number" name="staff_number" required>

    <label for="department">Department:</label>
    <input type="text" id="department" name="department" required>

    <label for="phone_number">Phone Number:</label>
    <input type="tel" id="phone_number" name="phone_number" required>

    <label for="designation">Designation:</label>
    <input type="text" id="designation" name="designation" required>

    <div class="upload-area">
        <label for="passport">Upload Passport Photo:</label>
        <input type="file" id="passport" name="passport" accept="image/*" required>
    </div>

    <div class="upload-area">
        <label for="signature">Upload Signature:</label>
        <input type="file" id="signature" name="signature" accept="image/*" required>
    </div>

    <button type="submit">Generate ID Card</button>
</form>

</body>
</html>
