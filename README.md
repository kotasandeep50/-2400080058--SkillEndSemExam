<!DOCTYPE html>
<html>
<head>
    <title>Live Student Search</title>
    <style>
        body {
            font-family: Arial;
            padding: 20px;
        }
        input {
            padding: 8px;
            width: 300px;
            margin-bottom: 10px;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        li {
            padding: 8px;
            border-bottom: 1px solid #ccc;
        }
    </style>
</head>
<body>

<h2>Live Search Filter - Student List</h2>

<input type="text" id="searchInput" placeholder="Search by Name or Roll No..." onkeyup="searchStudent()">

<ul id="studentList">
    <li>101 - Rahul</li>
    <li>102 - Suresh</li>
    <li>103 - Anjali</li>
    <li>104 - Priya</li>
    <li>105 - Kiran</li>
</ul>

<script>
function searchStudent() {
    let input = document.getElementById("searchInput").value.toLowerCase();
    let students = document.getElementById("studentList").getElementsByTagName("li");

    for (let i = 0; i < students.length; i++) {
        let text = students[i].textContent.toLowerCase();
        if (text.includes(input)) {
            students[i].style.display = "";
        } else {
            students[i].style.display = "none";
        }
    }
}
</script>

</body>
</html>
<!DOCTYPE html>
<html>
<head>
    <title>Live Student Search</title>
    <style>
        body {
            font-family: Arial;
            padding: 20px;
        }
        input {
            padding: 8px;
            width: 300px;
            margin-bottom: 10px;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        li {
            padding: 8px;
            border-bottom: 1px solid #ccc;
        }
    </style>
</head>
<body>

<h2>Live Search Filter - Student List</h2>

<input type="text" id="searchInput" placeholder="Search by Name or Roll No..." onkeyup="searchStudent()">

<ul id="studentList">
    <li>101 - Rahul</li>
    <li>102 - Suresh</li>
    <li>103 - Anjali</li>
    <li>104 - Priya</li>
    <li>105 - Kiran</li>
</ul>

<script>
function searchStudent() {
    let input = document.getElementById("searchInput").value.toLowerCase();
    let students = document.getElementById("studentList").getElementsByTagName("li");

    for (let i = 0; i < students.length; i++) {
        let text = students[i].textContent.toLowerCase();
        if (text.includes(input)) {
            students[i].style.display = "";
        } else {
            students[i].style.display = "none";
        }
    }
}
</script>

</body>
</html>
