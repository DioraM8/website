<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Assignment Submission</title>
<style>
body {
font-family: 'Poppins', sans-serif;
margin: 0;
padding: 0;
background: linear-gradient(135deg, #3A1C71, #D76D77, #FFAF7B);
text-align: center;
display: flex;
flex-direction: column;
align-items: center;
justify-content: center;
height: 100vh;
}
.container {
max-width: 500px;
background: rgba(255, 255, 255, 0.98);
padding: 25px;
border-radius: 15px;
box-shadow: 10px 10px 30px rgba(0, 0, 0, 0.3);
transform: perspective(1000px) rotateX(5deg);
transition: transform 0.3s ease-in-out;
}
.container:hover {
transform: perspective(1000px) rotateX(0deg);
}
h2 {
text-align: center;
color: #333;
font-size: 28px;
text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2);
}
label {
font-weight: bold;
display: block;
margin-top: 12px;
color: #444;
}
input, button {
width: 100%;
padding: 12px;
margin-top: 10px;
border-radius: 8px;
border: none;
box-shadow: inset 0 1px 5px rgba(0, 0, 0, 0.1);
font-size: 14px;
}
button {
background: linear-gradient(90deg, #6a11cb, #2575fc);
color: white;
font-size: 16px;
font-weight: bold;
cursor: pointer;
transition: background 0.3s ease-in-out, transform 0.2s;
box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.3);
}
button:hover {
background: linear-gradient(90deg, #5a0fc8, #1f5cc9);
transform: scale(1.1);
}
.header {
background: rgba(0, 0, 0, 0.85);
color: white;
padding: 20px;
font-size: 26px;
font-weight: bold;
text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
border-radius: 10px;
margin-bottom: 20px;
}
.file-info {
margin-top: 5px;
font-size: 12px;
color: #666;
}
</style>
</head>
<body>
<div class="header">Assignment Submission</div>
<div class="container">
<h2>Submit Your Assignment</h2>
<p><strong>Name:</strong> Muslimova Diyorakhon</p>
<p><strong>Student ID:</strong> 2417494</p>
<form action="#" method="post" enctype="multipart/form-data">
<label for="title">Assignment Title:</label>
<input type="text" id="title" name="title" required>
<label for="due-date">Due Date:</label>
<input type="date" id="due-date" name="due-date" required>
<label for="file">Upload File (All Document Types Accepted):</label>
<input type="file" id="file" name="file" required>
<div class="file-info">You can upload any document type: PDF, DOCX, PPTX, TXT, ZIP, RAR, etc.</div>
<button type="submit">Submit Assignment</button>
</form>
</div>
</body>
</html>
