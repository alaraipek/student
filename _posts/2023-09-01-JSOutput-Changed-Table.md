---
title: Table
comments: false
toc: true
layout: post
description: Defining when to use the right web language for your table.
courses: { compsci: {week: 2} }
type: hacks
---

## Markdown, HTML, and JavaScript: How Do They Compare and When to Use Each?
<!--1. Describe a benefit of a markdown table 2. Describe the difference between HTML and JavaScript 3. Describe a benefit of a table that uses JavaScript-->

Markdown, HTML, and JavaScript are all good web language options, but knowing when to use each is essential. Markdown is a markup language. Markup languages make coding in HTML easier for writers by simplifying tags and syntax. Coding beginners and web writers, especially journalists, find markdown tables ideal because Markdown's straightforward syntax makes their code more readable. **Therefore, one benefit of a markdown table is that it's organized and easier to interprate.** As a result, there is a lesser need for comments as well. Accompanied by Markdown, HTML and JavaScript are strictly designed for coding. **However, what sets JavaScript apart from HTML is that it provides interactivity.** For instance, the JavaScript table allows a user to input a search and be presented an output of related results. However, HTML does not include tags which enable this feature. **Therefore, a benefit of using JavaScript for tables is that it enables coders to utilize interaction.**

## Markdown Table

### Favorite Books

| Title                   | Genre       |
|  ------------           | ----------- |
| Where The Crawdads Sing | Fiction     |
| The Old Man and The Sea | Fiction     |

## HTML Table

### Favorite Books & Ratings

<!--CSS Styling, table & hover-->

<html>
<head>
<style>
table, th, td {
  border: 1px solid white;
  border-collapse: collapse;
}
th, td {
  background-color: #96D4D4;
}
tr:hover {background-color: #D6EEEE;}
</html>
</head>

<table class="table">
    <thead>
        <tr>
            <th>Title</th>
            <th>Author</th>
            <th>Note</th>
            <th>Star Ranking</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Where the Crawdads Sing</td>
            <td>Delia Owens</td>
            <td>Poetic fiction, prejudice & self-reliance </td>
            <td>★★★★★</td>
        </tr>
        <tr>
            <td>The Old Man and the Sea</td>
            <td>Ernest Hemmingway</td>
            <td>Fiction, struggle, resilience, & patience</td>
            <td>★★★★☆</td>
        </tr>
        <tr>
            <td>Moby Dick</td>
            <td>Herman Melville</td>
            <td>Adventure Fiction, survival & imperialism</td>
            <td>★★★★☆</td>
        </tr>
        <tr>
            <td>Harry Potter and the Sorcerer's Stone</td>
            <td>J.K. Rowling</td>
            <td>Fantasy, bravery & mystery</td>
            <td>★★★★★</td>
        </tr>
        <tr>
            <td>Just Kids</td>
            <td>Patti Smith</td>
            <td>Memoir, creativity & love</td>
            <td>★★★★★</td>
        </tr>
        <tr>
            <td>Atomic Habits</td>
            <td>James Clear</td>
            <td>Self-help/Self-Improvement</td>
            <td>★★★★☆</td>
        </tr>
        <tr>
            <td>The Great Gatsby</td>
            <td>F. Scott Fitzgerald</td>
            <td>Novel, tragedy & love</td>
            <td>★★★☆☆</td>
        </tr>
        <tr>
            <td>The Alchemist</td>
            <td>Paulo Coelho</td>
            <td>Adventure fiction, love/life lessons</td>
            <td>★★★★☆</td>
        </tr>
    </tbody>
</table>

## JavaScript Table

### Favorite Books Archive

<!-- Head contains information to Support the Document -->
<head>
    <!-- load jQuery and DataTables output style and scripts -->
    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.13.4/css/jquery.dataTables.min.css">
    <script type="text/javascript" language="javascript" src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script>var define = null;</script>
    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/1.13.4/js/jquery.dataTables.min.js"></script>
</head>

<!-- Body contains the contents of the Document -->
<body>
    <table id="demo" class="table">
    <thead>
        <tr>
            <th>Title</th>
            <th>Author</th>
            <th>Note</th>
            <th>Star Ranking</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Where the Crawdads Sing</td>
            <td>Delia Owens</td>
            <td>Poetic fiction, prejudice & self-reliance </td>
            <td>★★★★★</td>
        </tr>
        <tr>
            <td>The Old Man and the Sea</td>
            <td>Ernest Hemmingway</td>
            <td>Fiction, struggle, resilience, & patience</td>
            <td>★★★★☆</td>
        </tr>
        <tr>
            <td>Moby Dick</td>
            <td>Herman Melville</td>
            <td>Adventure Fiction, survival & imperialism</td>
            <td>★★★★☆</td>
        </tr>
        <tr>
            <td>Harry Potter and the Sorcerer's Stone</td>
            <td>J.K. Rowling</td>
            <td>Fantasy, bravery & mystery</td>
            <td>★★★★★</td>
        </tr>
        <tr>
            <td>Just Kids</td>
            <td>Patti Smith</td>
            <td>Memoir, creativity & love</td>
            <td>★★★★★</td>
        </tr>
        <tr>
            <td>Atomic Habits</td>
            <td>James Clear</td>
            <td>Self-help/Self-Improvement</td>
            <td>★★★★☆</td>
        </tr>
        <tr>
            <td>The Great Gatsby</td>
            <td>F. Scott Fitzgerald</td>
            <td>Novel, tragedy & love</td>
            <td>★★★☆☆</td>
        </tr>
        <tr>
            <td>The Alchemist</td>
            <td>Paulo Coelho</td>
            <td>Adventure fiction, love/life lessons</td>
            <td>★★★★☆</td>
        </tr>
    </tbody>
    </table>
</body>

<!-- Script is used to embed executable code -->
<script>
    $("#demo").DataTable();
</script>

## Future Hacks

The archived books list I designed is similar to how a library would show their inventory online. If this were a more useful website similar to that of a library, I would most likely want to add a hyperlink or dropdown page for each book, giving a rating section for readers to interact and share their ratings. Finally, the ratings would be averaged to list the final star rating.

#!pip install emoji
from emoji import emojize 
print(emojize(":thumbs_up: Python is awesome! :grinning_face:"))
