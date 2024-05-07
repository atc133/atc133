<!DOCTYPE html>
<html>
  <head> 
    <title>Job Application Form</title>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
   
  </head>
    <main>
      <h1>Job Application Form</h1>
      <form action="submit.php" method="post" enctype="multipart/form-data"></form>
        <div class="form-row">
          <label for="name">Name:</label>
          <input type="text" id="name" name="name"  placeholder="John Johnson"  required />
        </div>
        <div class="form-row">
          <label for="city">City:</label>
          <input type="text" id="city" name="city" placeholder="z.B.. Berlin" required />
        </div>
        <div class="form-row">
          <label for="email">Email:</label>
          <input type="email" id="email" name="email" placeholder="example@domain.de" required />
        </div>
        <div class="form-row">
          <label for="english">English:</label>
          <label><input type="radio" name="english" value="Very good" required /> Very Good</label>
          <label><input type="radio" name="english" value="Good" required /> Good</label>
          <label><input type="radio" name="english" value="None" required /> None</label>
        </div>
        <div class="form-row">
          <label for="german">German:</label>
          <label><input type="radio" name="german" value="Mother Tongue" required /> Mother Tongue</label>
          <label><input type="radio" name="german" value="Very good" required /> Very Good</label>
          <label><input type="radio" name="german" value="Good" required /> Good</label>
        </div>
        <div class="form-row">
          <label for="file">Upload your CV:</label>
          <input type="file" id="file" name="file" accept=".pdf,.doc,.docx" required />
        </div>
        <div class="form-row">
          <label for="message">Say something about yourself:</label>
          <textarea id="message" name="message"  placeholder="Please tell us why you're a good fit for this position and why you want to work with us" cols="24" rows="10" ></textarea>
        </div>
        <div class="form-Sumbit">
          <input type="submit" value="Send Application" />
        </div>
      </form>
    </main>
  <style>
    
    h1 {text-align: center;}
    .form-Sumbit {text-align: center;}
    main {
      background-color: #f5f5f5;
      padding: 50px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    .form-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 30px;
    }

    label {
      display: inline-block;
      width: 100px;
      text-align: right;
      font-size: 16px;
      font-weight: bold;
      color: #333;
    }

    input[type="text"],
    input[type="email"],
    textarea {
      flex-grow: 1;
      margin-left: 10px;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 16px;
      line-height: 1.5;
    }

    input[type="file"] {
      flex-grow: 1;
      margin-left: 10px;
      padding: 10px;
      border: 1px solid #ccc;
    }

    </style>
    
</html>
