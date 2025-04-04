<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">

<!-- Begin Jekyll SEO tag v2.8.0 -->
<meta name="generator" content="Jekyll v3.10.0" />
<meta property="og:title" content="github" />
<meta property="og:locale" content="en_US" />
<link rel="canonical" href="https://dioram8.github.io/github/" />
<meta property="og:url" content="https://dioram8.github.io/github/" />
<meta property="og:site_name" content="github" />
<meta property="og:type" content="website" />
<meta name="twitter:card" content="summary" />
<meta property="twitter:title" content="github" />
<script type="application/ld+json">
{"@context":"https://schema.org","@type":"WebSite","headline":"github","name":"github","url":"https://dioram8.github.io/github/"}</script>
<!-- End Jekyll SEO tag -->

    <link rel="stylesheet" href="/github/assets/css/style.css?v=13f5e9734754c9d25cdbfa0c62929168016c18a2">
    <!-- start custom head snippets, customize with your own _includes/head-custom.html file -->

<!-- Setup Google Analytics -->



<!-- You can set your favicon here -->
<!-- link rel="shortcut icon" type="image/x-icon" href="/github/favicon.ico" -->

<!-- end custom head snippets -->

  </head>
  <body>
    <div class="container-lg px-3 my-5 markdown-body">
      
      <h1><a href="https://dioram8.github.io/github/">github</a></h1>
      

<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Diyora's Assignment Portal</title>
    <link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700&amp;display=swap" rel="stylesheet" />
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Syne', sans-serif;
        }
        
        /* Upload styles */
        .upload-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 25px;
        }
        
        .file-upload-wrapper {
            width: 100%;
            max-width: 500px;
            position: relative;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .file-upload-label {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            width: 100%;
            height: 180px;
            border: 2px dashed rgba(167, 112, 255, 0.4);
            border-radius: 16px;
            background: rgba(255, 255, 255, 0.03);
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .file-upload-label:hover {
            border-color: #a770ff;
            background: rgba(255, 255, 255, 0.05);
            transform: translateY(-3px);
        }
        
        .upload-icon {
            font-size: 40px;
            color: #a770ff;
            margin-bottom: 10px;
        }
        
        .upload-text {
            font-size: 16px;
            color: rgba(255, 255, 255, 0.7);
        }
        
        .file-upload-input {
            position: absolute;
            width: 0.1px;
            height: 0.1px;
            opacity: 0;
            overflow: hidden;
            z-index: -1;
        }
        
        .file-info {
            margin-top: 15px;
            padding: 10px;
            color: rgba(255, 255, 255, 0.8);
            font-size: 14px;
            width: 100%;
            text-align: center;
            min-height: 20px;
        }
        
        .upload-options {
            display: flex;
            flex-direction: column;
            gap: 15px;
            width: 100%;
            max-width: 500px;
        }
        
        .assignment-select {
            width: 100%;
            padding: 14px;
            border-radius: 12px;
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            color: white;
            font-size: 16px;
            outline: none;
            transition: all 0.3s ease;
            appearance: none;
            background-image: linear-gradient(45deg, transparent 50%, #a770ff 50%), 
                            linear-gradient(135deg, #a770ff 50%, transparent 50%);
            background-position: calc(100% - 20px) calc(1em + 2px), 
                               calc(100% - 15px) calc(1em + 2px);
            background-size: 5px 5px, 5px 5px;
            background-repeat: no-repeat;
        }
        
        .assignment-select:hover, .assignment-select:focus {
            border-color: #a770ff;
            background-color: rgba(255, 255, 255, 0.08);
        }
        
        .assignment-select option {
            background-color: #0f0f1e;
            color: white;
        }
        
        .upload-button {
            padding: 15px;
            background: linear-gradient(90deg, #a770ff, #cf8fff);
            border: none;
            border-radius: 12px;
            color: white;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            letter-spacing: 0.5px;
            box-shadow: 0 5px 15px rgba(167, 112, 255, 0.3);
        }
        
        .upload-button:hover {
            background: linear-gradient(90deg, #cf8fff, #a770ff);
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(167, 112, 255, 0.4);
        }
        
        body {
            background: #0f0f1e;
            background-image: 
                radial-gradient(circle at 20% 30%, rgba(76, 0, 255, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 80% 70%, rgba(255, 0, 128, 0.15) 0%, transparent 50%);
            color: white;
            text-align: center;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            overflow-x: hidden;
        }
        
        .navbar {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 25px;
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(12px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            position: relative;
            z-index: 10;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .navbar h1 {
            font-size: 24px;
            letter-spacing: 2px;
            font-weight: 600;
            text-transform: uppercase;
            background: linear-gradient(90deg, #f0f0f0, #a770ff);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
        }
        
        .container {
            max-width: 1100px;
            margin: 60px auto;
            display: flex;
            flex-direction: column;
            gap: 40px;
            padding: 0 30px;
            flex-grow: 1;
            position: relative;
        }
        
        .card {
            background: rgba(15, 15, 30, 0.5);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.25);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            border: 1px solid rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            position: relative;
        }
        
        .card::before {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            background: linear-gradient(45deg, #ff00cc, #3333ff, #00ffff, #ff00cc);
            z-index: -1;
            border-radius: 21px;
            background-size: 400%;
            opacity: 0;
            transition: opacity 0.4s ease;
        }
        
        .card:hover {
            transform: translateY(-10px);
        }
        
        .card:hover::before {
            opacity: 0.5;
            animation: glowingBorder 8s linear infinite;
        }
        
        @keyframes glowingBorder {
            0% { background-position: 0 0; }
            50% { background-position: 400% 0; }
            100% { background-position: 0 0; }
        }
        
        .card-header {
            background: rgba(0, 0, 0, 0.2);
            color: white;
            padding: 25px 30px;
            font-size: 22px;
            font-weight: 700;
            letter-spacing: 1px;
            position: relative;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .card-header::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
        }
        
        .card-body {
            padding: 35px;
            color: rgba(255, 255, 255, 0.8);
        }
        
        /* Assignment Section Styles */
        .assignment-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 30px;
            margin-top: 25px;
        }
        
        .assignment-item {
            background: rgba(255, 255, 255, 0.03);
            border-radius: 16px;
            padding: 15px;
            transition: all 0.5s cubic-bezier(0.19, 1, 0.22, 1);
            position: relative;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100px;
            border: 1px solid rgba(255, 255, 255, 0.02);
            box-shadow: 0 7px 20px rgba(0, 0, 0, 0.1);
        }
        
        .assignment-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 4px;
            height: 0;
            background: linear-gradient(to bottom, #ff00cc, #3333ff);
            transition: height 0.5s ease;
        }
        
        .assignment-item:hover {
            background: rgba(255, 255, 255, 0.05);
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }
        
        .assignment-item:hover::before {
            height: 100%;
        }
        
        .assignment-link {
            color: #a770ff;
            text-decoration: none;
            font-size: 18px;
            font-weight: 600;
            position: relative;
            transition: all 0.3s ease;
            padding-bottom: 3px;
            letter-spacing: 0.5px;
            background: linear-gradient(90deg, #fff, #a770ff);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100%;
        }
        
        .assignment-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            background: linear-gradient(90deg, #a770ff, #cf8fff);
            transition: width 0.3s ease;
        }
        
        .assignment-link:hover {
            text-shadow: 0 0 8px rgba(167, 112, 255, 0.5);
        }
        
        .assignment-link:hover::after,
        .assignment-link.uploaded::after {
            width: 80%;
        }
        
        .assignment-item.active {
            border-color: rgba(167, 112, 255, 0.5);
            background: rgba(167, 112, 255, 0.1);
        }
        
        .assignment-item.active::before {
            height: 100%;
        }
        
        footer {
            background: rgba(0, 0, 0, 0.3);
            padding: 20px;
            text-align: center;
            margin-top: auto;
            font-size: 14px;
            letter-spacing: 1px;
            color: rgba(255, 255, 255, 0.5);
            backdrop-filter: blur(10px);
            border-top: 1px solid rgba(255, 255, 255, 0.03);
        }
        
        /* Decorative elements */
        .glow-circle {
            position: absolute;
            border-radius: 50%;
            filter: blur(60px);
            z-index: -1;
            opacity: 0.25;
        }
        
        .glow-1 {
            width: 400px;
            height: 400px;
            background: #ff00cc;
            top: -100px;
            right: -100px;
        }
        
        .glow-2 {
            width: 350px;
            height: 350px;
            background: #3333ff;
            bottom: 10%;
            left: -100px;
        }
        
        /* Animation for cards */
        @keyframes floatAnimation {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
    </style>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Handle file upload UI
            const fileUpload = document.getElementById('fileUpload');
            const fileInfo = document.getElementById('fileInfo');
            const uploadButton = document.getElementById('uploadButton');
            const assignmentSelect = document.getElementById('assignmentNumber');
            
            // Update file info when a file is selected
            fileUpload.addEventListener('change', function() {
                if (this.files && this.files[0]) {
                    const file = this.files[0];
                    const fileSizeInMB = (file.size / (1024 * 1024)).toFixed(2);
                    fileInfo.innerHTML = `<span style="color: #a770ff">${file.name}</span> (${fileSizeInMB} MB)`;
                } else {
                    fileInfo.textContent = '';
                }
            });
            
            // Handle upload button click
            uploadButton.addEventListener('click', function() {
                if (!fileUpload.files || !fileUpload.files[0]) {
                    alert('Please select a file to upload');
                    return;
                }
                
                if (!assignmentSelect.value) {
                    alert('Please select an assignment number');
                    return;
                }
                
                // In a real implementation, this would send the file to a server
                // For this demo, we'll simulate a successful upload
                uploadButton.textContent = 'Uploading...';
                uploadButton.disabled = true;
                
                setTimeout(() => {
                    alert(`Assignment ${assignmentSelect.value} uploaded successfully!`);
                    fileInfo.textContent = '';
                    assignmentSelect.value = '';
                    fileUpload.value = '';
                    uploadButton.textContent = 'Upload';
                    uploadButton.disabled = false;
                    
                    // Update the corresponding assignment link to indicate it has content
                    const assignmentLinks = document.querySelectorAll('.assignment-link');
                    const assignmentNumber = parseInt(assignmentSelect.value) - 1;
                    
                    if (assignmentLinks[assignmentNumber]) {
                        assignmentLinks[assignmentNumber].classList.add('uploaded');
                        assignmentLinks[assignmentNumber].parentElement.classList.add('active');
                    }
                }, 2000);
            });
        });
    </script>
</head>
<body>
    <div class="navbar">
        <h1>Diyora - Student No: 2417494</h1>
    </div>
    
    <div class="container">
        <!-- Decorative elements -->
        <div class="glow-circle glow-1"></div>
        <div class="glow-circle glow-2"></div>
        
        <!-- Assignments Section -->
        <!-- Upload Section -->
        <div class="card">
            <div class="card-header">Upload Assignment</div>
            <div class="card-body">
                <div class="upload-container">
                    <form id="uploadForm" enctype="multipart/form-data">
                        <div class="file-upload-wrapper">
                            <label for="fileUpload" class="file-upload-label">
                                <span class="upload-icon">+</span>
                                <span class="upload-text">Select assignment file</span>
                            </label>
                            <input type="file" id="fileUpload" name="assignmentFile" class="file-upload-input" />
                            <div id="fileInfo" class="file-info"></div>
                        </div>
                        <div class="upload-options">
                            <select id="assignmentNumber" name="assignmentNumber" class="assignment-select">
                                <option value="" disabled="" selected="">Select assignment number</option>
                                <option value="1">Assignment 1</option>
                                <option value="2">Assignment 2</option>
                                <option value="3">Assignment 3</option>
                                <option value="4">Assignment 4</option>
                                <option value="5">Assignment 5</option>
                                <option value="6">Assignment 6</option>
                            </select>
                            <button type="button" id="uploadButton" class="upload-button">Upload</button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
        
        <!-- Assignment Collection Section -->
        <div class="card">
            <div class="card-header">Assignment Collection</div>
            <div class="card-body">
                <p>My Assignment Collection</p>
                
                <div class="assignment-list">
                    <div class="assignment-item">
                        <a href="https://docs.google.com/document/d/1z1v-lLQ0GKyZsSDASf-bf2dJ2qaiNxGvPdjN58VEEm0/edit?usp=drive_link" class="assignment-link">Assignment 1</a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="https://dioram8.github.io/assignment2/" class="assignment-link">Assignment 2</a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="https://dioram8.github.io/assignment3/" class="assignment-link">Assignment 3</a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="https://drive.google.com/drive/folders/1NiWr6MC1IktlPcXPBEHMnrXVkMK0a1eC?usp=drive_link" class="assignment-link">Assignment 4</a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="https://drive.google.com/drive/folders/1NiWr6MC1IktlPcXPBEHMnrXVkMK0a1eC?usp=drive_link" class="assignment-link">Assignment 5</a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="https://drive.google.com/drive/folders/1NiWr6MC1IktlPcXPBEHMnrXVkMK0a1eC?usp=drive_link" class="assignment-link">Assignment 6</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <footer>
        &copy; 2025 Diyora | Dong-A University
    </footer>
</body>
</html>


      
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/anchor-js/4.1.0/anchor.min.js" integrity="sha256-lZaRhKri35AyJSypXXs4o6OPFTbTmUoltBbDCbdzegg=" crossorigin="anonymous"></script>
    <script>anchors.add();</script>
  </body>
</html>
