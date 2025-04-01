# welcome to image-compressor

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Free online tool to compress your images while maintaining quality. Reduce file size for JPG, PNG, and WebP images.">
    <meta name="keywords" content="image compressor, reduce image size, optimize images, online image tool, photo compressor">
    <meta name="author" content="Image Compressor Tool">
    <meta property="og:title" content="Free Online Image Compression Tool">
    <meta property="og:description" content="Compress your images easily without losing quality. Perfect for web optimization.">
    <meta property="og:type" content="website">
    <meta name="robots" content="index, follow">
    
    <title>Free Online Image Compression Tool | Optimize Your Photos</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- AdMob SDK -->
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=google.com, pub-3535001234721478, DIRECT, f08c47fec0942fa0 crossorigin="anonymous"></script>
    
    <style>
        :root {
            --primary-color: #4361ee;
            --secondary-color: #3f37c9;
            --accent-color: #4895ef;
            --light-color: #f8f9fa;
            --dark-color: #212529;
            --gray-color: #6c757d;
            --success-color: #4bb543;
            --error-color: #ff3333;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--dark-color);
            background-color: #f5f7ff;
            padding: 0;
            margin: 0;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 24px;
            font-weight: 700;
            color: var(--primary-color);
            text-decoration: none;
        }
        
        .logo span {
            color: var(--accent-color);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 20px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--dark-color);
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--primary-color);
        }
        
        .hero {
            text-align: center;
            padding: 60px 0 40px;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: var(--dark-color);
        }
        
        .hero p {
            font-size: 1.1rem;
            color: var(--gray-color);
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        .ad-banner {
            background-color: #f0f0f0;
            border: 1px dashed #ccc;
            padding: 20px;
            text-align: center;
            margin: 30px 0;
            border-radius: 5px;
        }
        
        .compressor-container {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            padding: 30px;
            margin-bottom: 40px;
        }
        
        .upload-area {
            border: 2px dashed var(--gray-color);
            border-radius: 8px;
            padding: 40px 20px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            margin-bottom: 30px;
            position: relative;
        }
        
        .upload-area:hover {
            border-color: var(--primary-color);
            background-color: rgba(67, 97, 238, 0.05);
        }
        
        .upload-area.active {
            border-color: var(--success-color);
            background-color: rgba(75, 181, 67, 0.05);
        }
        
        .upload-area i {
            font-size: 48px;
            color: var(--primary-color);
            margin-bottom: 15px;
        }
        
        .upload-area h3 {
            margin-bottom: 10px;
            color: var(--dark-color);
        }
        
        .upload-area p {
            color: var(--gray-color);
            margin-bottom: 20px;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--primary-color);
            color: white;
            padding: 12px 24px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 500;
            border: none;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: var(--secondary-color);
        }
        
        .btn-outline {
            background-color: transparent;
            border: 1px solid var(--primary-color);
            color: var(--primary-color);
        }
        
        .btn-outline:hover {
            background-color: var(--primary-color);
            color: white;
        }
        
        .settings {
            margin-bottom: 30px;
        }
        
        .settings h3 {
            margin-bottom: 15px;
            color: var(--dark-color);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }
        
        input[type="range"] {
            width: 100%;
            height: 8px;
            -webkit-appearance: none;
            background: #e0e0e0;
            border-radius: 5px;
            outline: none;
        }
        
        input[type="range"]::-webkit-slider-thumb {
            -webkit-appearance: none;
            width: 20px;
            height: 20px;
            background: var(--primary-color);
            border-radius: 50%;
            cursor: pointer;
        }
        
        .range-value {
            display: inline-block;
            width: 40px;
            text-align: center;
            font-weight: 600;
            color: var(--primary-color);
        }
        
        select {
            width: 100%;
            padding: 10px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-family: inherit;
            font-size: 16px;
            background-color: white;
        }
        
        .preview-container {
            display: none;
            margin-top: 30px;
        }
        
        .preview-row {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .preview-col {
            flex: 1;
            min-width: 300px;
        }
        
        .preview-card {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
            padding: 20px;
            height: 100%;
        }
        
        .preview-card h4 {
            margin-bottom: 15px;
            color: var(--dark-color);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .preview-card .badge {
            background-color: var(--accent-color);
            color: white;
            padding: 3px 10px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: 500;
        }
        
        .image-preview {
            width: 100%;
            height: auto;
            max-height: 300px;
            object-fit: contain;
            margin-bottom: 15px;
            border-radius: 5px;
        }
        
        .file-info {
            font-size: 14px;
            color: var(--gray-color);
        }
        
        .file-info div {
            margin-bottom: 5px;
            display: flex;
            justify-content: space-between;
        }
        
        .file-info span {
            font-weight: 500;
            color: var(--dark-color);
        }
        
        .action-btns {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .action-btns .btn {
            flex: 1;
            text-align: center;
            padding: 10px;
        }
        
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 40px 0 20px;
            margin-top: 60px;
        }
        
        .footer-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 30px;
        }
        
        .footer-col {
            flex: 1;
            min-width: 250px;
        }
        
        .footer-col h3 {
            color: white;
            margin-bottom: 20px;
            font-size: 18px;
        }
        
        .footer-col ul {
            list-style: none;
        }
        
        .footer-col ul li {
            margin-bottom: 10px;
        }
        
        .footer-col ul li a {
            color: #adb5bd;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-col ul li a:hover {
            color: white;
        }
        
        .copyright {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #adb5bd;
            font-size: 14px;
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 20px;
                justify-content: center;
            }
            
            nav ul li {
                margin: 0 10px;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .preview-row {
                flex-direction: column;
            }
            
            .action-btns {
                flex-direction: column;
            }
        }
        
        @media (max-width: 480px) {
            .hero {
                padding: 40px 0 20px;
            }
            
            .hero h1 {
                font-size: 1.8rem;
            }
            
            .compressor-container {
                padding: 20px 15px;
            }
            
            .upload-area {
                padding: 30px 15px;
            }
        }
        
        /* Loading spinner */
        .spinner {
            display: none;
            width: 40px;
            height: 40px;
            margin: 20px auto;
            border: 4px solid rgba(0, 0, 0, 0.1);
            border-radius: 50%;
            border-top: 4px solid var(--primary-color);
            animation: spin 1s linear infinite;
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        /* Progress bar */
        .progress-container {
            width: 100%;
            height: 8px;
            background-color: #f0f0f0;
            border-radius: 5px;
            margin: 20px 0;
            display: none;
        }
        
        .progress-bar {
            height: 100%;
            background-color: var(--primary-color);
            border-radius: 5px;
            width: 0%;
            transition: width 0.3s;
        }
    </style>
</head>
<body>
    <header>
        <div class="container header-content">
            <a href="#" class="logo">Image<span>Compressor</span></a>
            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">How It Works</a></li>
                    <li><a href="#">Features</a></li>
                    <li><a href="#">FAQ</a></li>
                </ul>
            </nav>
        </div>
    </header>
    
    <main class="container">
        <section class="hero">
            <h1>Compress Images Without Losing Quality</h1>
            <p>Reduce the file size of your JPG, PNG, and WebP images with our free online tool. Perfect for optimizing website performance and saving storage space.</p>
        </section>
        
        <!-- Banner Ad (Top) -->
        <div class="ad-banner">
            <script>
                (adsbygoogle = window.adsbygoogle || []).push({
                    google_ad_client: "ca-app-pub-3535001234721478/8188780502",
                    enable_page_level_ads: true
                });
            </script>
        </div>
        
        <section class="compressor-container">
            <div class="upload-area" id="uploadArea">
                <i>📁</i>
                <h3>Drag & Drop Your Images Here</h3>
                <p>or click to browse files (JPG, PNG, WebP supported)</p>
                <input type="file" id="fileInput" accept="image/jpeg,image/png,image/webp" style="display: none;">
                <button class="btn">Select Files</button>
            </div>
            
            <div class="settings">
                <h3>Compression Settings</h3>
                <div class="form-group">
                    <label for="quality">Quality: <span id="qualityValue" class="range-value">80</span>%</label>
                    <input type="range" id="quality" min="1" max="100" value="80">
                </div>
                
                <div class="form-group">
                    <label for="outputFormat">Output Format</label>
                    <select id="outputFormat">
                        <option value="original">Keep original format</option>
                        <option value="jpeg">JPEG</option>
                        <option value="png">PNG</option>
                        <option value="webp">WebP (recommended)</option>
                    </select>
                </div>
                
                <button id="compressBtn" class="btn" disabled>Compress Images</button>
                
                <div class="progress-container" id="progressContainer">
                    <div class="progress-bar" id="progressBar"></div>
                </div>
                
                <div class="spinner" id="spinner"></div>
            </div>
            
            <div class="preview-container" id="previewContainer">
                <h3>Results</h3>
                <div class="preview-row" id="previewRow">
                    <!-- Preview cards will be added here dynamically -->
                </div>
                
                <div class="action-btns">
                    <button id="downloadAllBtn" class="btn">Download All</button>
                    <button id="resetBtn" class="btn btn-outline">Reset</button>
                </div>
            </div>
        </section>
        
        <!-- Interstitial Ad (Middle) -->
        <div class="ad-banner">
            <script>
                (adsbygoogle = window.adsbygoogle || []).push({
                    google_ad_client: "ca-app-pub-3535001234721478/7558225115",
                    enable_page_level_ads: true
                });
            </script>
        </div>
        
        <section class="info-section">
            <h2>Why Compress Your Images?</h2>
            <p>Image compression is essential for faster website loading, reduced bandwidth usage, and improved user experience. Our tool helps you find the perfect balance between quality and file size.</p>
            
            <h3>How It Works</h3>
            <ol>
                <li>Upload your images (drag & drop or click to browse)</li>
                <li>Adjust compression settings to your preference</li>
                <li>Click "Compress Images" and wait a few seconds</li>
                <li>Download your optimized images</li>
            </ol>
        </section>
    </main>
    
    <!-- Rewarded Ad (Bottom) -->
    <div class="container">
        <div class="ad-banner">
            <script>
                (adsbygoogle = window.adsbygoogle || []).push({
                    google_ad_client: "ca-app-pub-3535001234721478/6245143446",
                    enable_page_level_ads: true
                });
            </script>
        </div>
    </div>
    
    <footer>
        <div class="container footer-content">
            <div class="footer-col">
                <h3>ImageCompressor</h3>
                <p>Free online tool to optimize your images for web and mobile.</p>
            </div>
            <div class="footer-col">
                <h3>Quick Links</h3>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Terms of Service</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h3>Resources</h3>
                <ul>
                    <li><a href="#">Image Optimization Guide</a></li>
                    <li><a href="#">Web Performance Tips</a></li>
                    <li><a href="#">Developer API</a></li>
                </ul>
            </div>
        </div>
        <div class="container copyright">
            <p>&copy; <span id="year"></span> ImageCompressor Tool. All rights reserved.</p>
        </div>
    </footer>
    
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Set current year in footer
            document.getElementById('year').textContent = new Date().getFullYear();
            
            // DOM elements
            const uploadArea = document.getElementById('uploadArea');
            const fileInput = document.getElementById('fileInput');
            const qualitySlider = document.getElementById('quality');
            const qualityValue = document.getElementById('qualityValue');
            const outputFormat = document.getElementById('outputFormat');
            const compressBtn = document.getElementById('compressBtn');
            const previewContainer = document.getElementById('previewContainer');
            const previewRow = document.getElementById('previewRow');
            const downloadAllBtn = document.getElementById('downloadAllBtn');
            const resetBtn = document.getElementById('resetBtn');
            const spinner = document.getElementById('spinner');
            const progressContainer = document.getElementById('progressContainer');
            const progressBar = document.getElementById('progressBar');
            
            // Global variables
            let files = [];
            let compressedFiles = [];
            
            // Update quality value display
            qualitySlider.addEventListener('input', function() {
                qualityValue.textContent = this.value;
            });
            
            // Upload area click event
            uploadArea.addEventListener('click', function() {
                fileInput.click();
            });
            
            // File input change event
            fileInput.addEventListener('change', function(e) {
                if (e.target.files.length > 0) {
                    files = Array.from(e.target.files);
                    updateUI();
                }
            });
            
            // Drag and drop events
            uploadArea.addEventListener('dragover', function(e) {
                e.preventDefault();
                uploadArea.classList.add('active');
            });
            
            uploadArea.addEventListener('dragleave', function() {
                uploadArea.classList.remove('active');
            });
            
            uploadArea.addEventListener('drop', function(e) {
                e.preventDefault();
                uploadArea.classList.remove('active');
                
                if (e.dataTransfer.files.length > 0) {
                    files = Array.from(e.dataTransfer.files).filter(file => 
                        file.type.match('image/jpeg') || 
                        file.type.match('image/png') || 
                        file.type.match('image/webp')
                    );
                    updateUI();
                }
            });
            
            // Compress button click event
            compressBtn.addEventListener('click', function() {
                if (files.length === 0) return;
                
                spinner.style.display = 'block';
                progressContainer.style.display = 'block';
                compressBtn.disabled = true;
                compressedFiles = [];
                
                // Process files with progress
                let processed = 0;
                const total = files.length;
                
                files.forEach((file, index) => {
                    compressImage(file, function(compressedFile) {
                        compressedFiles.push(compressedFile);
                        processed++;
                        
                        // Update progress
                        const progress = Math.round((processed / total) * 100);
                        progressBar.style.width = progress + '%';
                        
                        if (processed === total) {
                            // All files processed
                            spinner.style.display = 'none';
                            compressBtn.disabled = false;
                            showPreviews();
                        }
                    });
                });
            });
            
            // Reset button click event
            resetBtn.addEventListener('click', function() {
                files = [];
                compressedFiles = [];
                fileInput.value = '';
                previewContainer.style.display = 'none';
                compressBtn.disabled = true;
                progressContainer.style.display = 'none';
                progressBar.style.width = '0%';
            });
            
            // Download all button click event
            downloadAllBtn.addEventListener('click', function() {
                compressedFiles.forEach(file => {
                    downloadFile(file);
                });
            });
            
            // Update UI based on selected files
            function updateUI() {
                if (files.length > 0) {
                    compressBtn.disabled = false;
                } else {
                    compressBtn.disabled = true;
                }
            }
            
            // Compress image function
            function compressImage(file, callback) {
                const reader = new FileReader();
                reader.readAsDataURL(file);
                
                reader.onload = function(event) {
                    const img = new Image();
                    img.src = event.target.result;
                    
                    img.onload = function() {
                        const canvas = document.createElement('canvas');
                        const ctx = canvas.getContext('2d');
                        
                        // Calculate new dimensions if needed (maintain aspect ratio)
                        const MAX_WIDTH = 2000;
                        const MAX_HEIGHT = 2000;
                        let width = img.width;
                        let height = img.height;
                        
                        if (width > height) {
                            if (width > MAX_WIDTH) {
                                height *= MAX_WIDTH / width;
                                width = MAX_WIDTH;
                            }
                        } else {
                            if (height > MAX_HEIGHT) {
                                width *= MAX_HEIGHT / height;
                                height = MAX_HEIGHT;
                            }
                        }
                        
                        canvas.width = width;
                        canvas.height = height;
                        
                        // Draw image on canvas
                        ctx.drawImage(img, 0, 0, width, height);
                        
                        // Get output format
                        let format = outputFormat.value;
                        if (format === 'original') {
                            format = file.type.split('/')[1];
                        }
                        
                        // Quality setting
                        const quality = qualitySlider.value / 100;
                        
                        // Convert to blob
                        canvas.toBlob(function(blob) {
                            const compressedFile = new File([blob], getOutputFilename(file.name, format), {
                                type: `image/${format}`,
                                lastModified: Date.now()
                            });
                            
                            callback(compressedFile);
                        }, `image/${format}`, quality);
                    };
                };
            }
            
            // Generate output filename
            function getOutputFilename(filename, format) {
                const nameWithoutExt = filename.split('.').slice(0, -1).join('.');
                return `${nameWithoutExt}-compressed.${format}`;
            }
            
            // Show previews of compressed images
            function showPreviews() {
                previewRow.innerHTML = '';
                
                compressedFiles.forEach((file, index) => {
                    const reader = new FileReader();
                    reader.readAsDataURL(file);
                    
                    reader.onload = function() {
                        const originalFile = files[index];
                        
                        const previewCard = document.createElement('div');
                        previewCard.className = 'preview-col';
                        previewCard.innerHTML = `
                            <div class="preview-card">
                                <h4>Preview <span class="badge">${file.type.split('/')[1].toUpperCase()}</span></h4>
                                <img src="${reader.result}" alt="Compressed preview" class="image-preview">
                                <div class="file-info">
                                    <div>
                                        <span>Original:</span> ${formatFileSize(originalFile.size)}
                                    </div>
                                    <div>
                                        <span>Compressed:</span> ${formatFileSize(file.size)}
                                    </div>
                                    <div>
                                        <span>Reduction:</span> ${calculateReduction(originalFile.size, file.size)}
                                    </div>
                                </div>
                                <button class="btn download-btn" data-index="${index}">Download</button>
                            </div>
                        `;
                        
                        previewRow.appendChild(previewCard);
                    };
                });
                
                // Add event listeners to download buttons
                document.querySelectorAll('.download-btn').forEach(btn => {
                    btn.addEventListener('click', function() {
                        const index = parseInt(this.getAttribute('data-index'));
                        downloadFile(compressedFiles[index]);
                    });
                });
                
                previewContainer.style.display = 'block';
            }
            
            // Download file function
            function downloadFile(file) {
                const url = URL.createObjectURL(file);
                const a = document.createElement('a');
                a.href = url;
                a.download = file.name;
                document.body.appendChild(a);
                a.click();
                document.body.removeChild(a);
                URL.revokeObjectURL(url);
            }
            
            // Format file size
            function formatFileSize(bytes) {
                if (bytes === 0) return '0 Bytes';
                
                const k = 1024;
                const sizes = ['Bytes', 'KB', 'MB', 'GB'];
                const i = Math.floor(Math.log(bytes) / Math.log(k));
                
                return parseFloat((bytes / Math.pow(k, i)).toFixed(2)) + ' ' + sizes[i];
            }
            
            // Calculate reduction percentage
            function calculateReduction(originalSize, compressedSize) {
                const reduction = ((originalSize - compressedSize) / originalSize) * 100;
                return reduction.toFixed(2) + '%';
            }
        });
    </script>
</body>
</html>
