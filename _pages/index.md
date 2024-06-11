<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body, html {
            margin: 0;
            padding: 0;
            height: 100%;
            overflow-x: hidden;
            position: relative;
        }

        .background-image {
            position: absolute;
            top: 0;
            right: 0;
            width: 25%;
            height: 100%;
            background: url('profile.jpg') no-repeat center center;
            background-size: cover;
            z-index: -1;
        }

        .background-image::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(to right, rgba(255, 255, 255, 0) 0%, rgba(255, 255, 255, 1) 100%);
        }

        .content {
            padding: 20px;
            position: relative;
            z-index: 1;
        }
    </style>
</head>
<body>
    <div class="background-image"></div>
    <div class="content">
        <h1>Your Content Here</h1>
        <p>This is an example of a page with a right-aligned background image that fades at the edges.</p>
        <p>Add more content here to see the scroll effect. </p>
        <p>More content...</p>
        <p>More content...</p>
        <p>More content...</p>
        <p>More content...</p>
    </div>
</body>
</html>
