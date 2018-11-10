---
layout: page
title: Contact
comments: false
---
<html>
<head>
<style>
* {
    box-sizing: border-box;
}

input[type=text], select, textarea {
    width: 100%;
    padding: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
    resize: vertical;
}

input[type=submit] {
    background-color: #4C66AF;
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    float: right;
    box-shadow: 2px 2px 2px #203368;
}

input[type=submit]:hover {
    background-color: #4C70D5;
}

input[type=submit]:active {
    box-shadow: none;
}

.container {
    border-radius: 5px;
    background-color: #f2f2f2;
    padding: 20px;
}

/* Clear floats after the columns */
.row:after {
    content: "";
    display: table;
    clear: both;
}

}
</style>
</head>
<body>

<div class="container">
  <form action="{{ site.url }}/message-sent/" name="contact" netlify>
    <div class="row">
      <div>
        <input type="text" id="fname" name="First Name" placeholder="First Name">
      </div>
    </div>
    <div class="row">
      <div>
        <input type="text" id="lname" name="Last Name" placeholder="Last Name">
      </div>
    </div>
    <div class="row">
      <div>
        <input type="text" id="email" name="Email" placeholder="Email">
      </div>
    </div>
    <div class="row">
      <div>
        <textarea id="subject" name="Message" placeholder="Message" style="height:200px"></textarea>
      </div>
    </div>
    <div class="row">
      <input type="submit" value="Submit">
    </div>
    <input type="hidden" name="_gotcha"><!-- use this to prevent spam -->
  </form>
</div>

</body>
</html>
