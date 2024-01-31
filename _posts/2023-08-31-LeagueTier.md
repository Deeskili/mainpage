---
toc: false
comments: false
layout: post
title: League of Legends Tier List
description: Here is a current tier list of my favorite League of Legends Champions! 
type: tangibles
courses: { compsci: {week: 2} }
---


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
                <th>Champion</th>
                <th>Tier </th>
                <th>Role</th>
                <th>Auto Attack?</th>
                <th>Price</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Darius</td>
                <td>A</td>
                <td>Top</td>
                <td>Yes</td>
                <td>4800 BE</td>
            </tr>
            <tr>
                <td>Riven</td>
                <td>S</td>
                <td>Top</td>
                <td>Yes</td>
                <td>6300 BE</td>
            </tr>
            <tr>
                <td>Yone</td>
                <td>A</td>
                <td>Mid</td>
                <td>Yes</td>
                <td>4800 BE</td>
            </tr>
            <tr>
                <td>Amumu</td>
                <td>S</td>
                <td>Jungler</td>
                <td>No</td>
                <td>450 BE</td>
            </tr>
            <tr>
                <td>Zeri</td>
                <td>D</td>
                <td>Bottom</td>
                <td>Yes</td>
                <td>6300 BE</td>
            </tr>
            <tr>
                <td>Lux</td>
                <td>B</td>
                <td>Support</td>
                <td>No</td>
                <td>1350 BE</td>
            </tr>
            <tr>
                <td>Yasuo</td>
                <td>B</td>
                <td>Mid</td>
                <td>Yes</td>
                <td>450 BE</td>
            </tr>
            <tr>
                <td>Tristana</td>
                <td>C</td>
                <td>Bottom</td>
                <td>Yes</td>
                <td>450 BE</td>
            </tr>
            <tr>
                <td>Nautilus</td>
                <td>S+</td>
                <td>Support</td>
                <td>No</td>
                <td>1350 BE</td>
            </tr>
            <tr>
                <td>Zed</td>
                <td>A</td>
                <td>Mid</td>
                <td>Yes</td>
                <td>6300 BE</td>
            </tr>
            <tr>
                <td>Irelia</td>
                <td>B</td>
                <td>Mid</td>
                <td>Yes</td>
                <td>1350 BE</td>
            </tr>
        </tbody>
    </table>
</body>
Benefits of Markdown Chart: Very interactive, Lots of Features, including search menu, how many entries shown per page, etc <br>
If I wanted to improve this chart/table, I would make it so that each line would link to a website to improve accessibility

<script>
    $("#demo").DataTable();
</script>