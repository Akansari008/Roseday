# Roseday
<!DOCTYPE html>

<html lang="en">

  <head>

    <meta charset="UTF-8" />

    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

    <title>untoldcoding</title>

    <link rel="stylesheet" href="new.css" />

  </head>

  <body>

    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Rose Day!</title>
    <style>
        body {
            background-color: #fff0f3;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        .container {
            position: relative;
        }

        /* The Rose Petals */
        .rose {
            position: relative;
            width: 100px;
            height: 100px;
            background: #e63946;
            border-radius: 50% 50% 50% 50% / 40% 40% 60% 60%;
            animation: bloom 3s infinite alternate;
            box-shadow: inset 0 0 20px rgba(0,0,0,0.2);
        }

        .rose::before, .rose::after {
            content: '';
            position: absolute;
            background: #d00000;
            width: 100px;
            height: 100px;
            border-radius: 50%;
        }

        .rose::before { left: -30px; transform: rotate(-15deg); }
        .rose::after { right: -30px; transform: rotate(15deg); }

        /* The Stem */
        .stem {
            width: 10px;
            height: 150px;
            background: #2d6a4f;
            margin: -10px auto 0;
            border-radius: 5px;
            position: relative;
            z-index: -1;
        }

        /* The Leaf */
        .leaf {
            width: 40px;
            height: 20px;
            background: #40916c;
            border-radius: 20px 0;
            position: absolute;
            top: 50px;
            left: 10px;
            
