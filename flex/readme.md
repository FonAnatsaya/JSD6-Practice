HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Learn-Flex</title>
</head>

<body>
    <!-- <h1>Learn-Flex</h1> -->

    <div class="flex-parent">
        <div class="flex-children">child-1</div>
        <div class="flex-children">child-2</div>
        <div class="flex-children">child-3</div>
        <div class="flex-children">child-4</div>
    </div>
</body>

</html>



css

* {
margin: 0;
padding: 0;
box-sizing: border-box;
}

/* the box size is wrapped and adjusted the size of the words of children as same as the box size */
.flex-parent {
/* Set height only when the screen covered 100% is needed. For row is 100% by default, then no need to set height100%*/
height: 10vh;
background-color: wheat;
display: flex;

/* //specify which axis will be the main one >> this case the main axia is row(L --> R) , and justify-content is used
not the align-item*/
/* flex-direction: row;

justify-content: space-around; */
gap: 20px;
/* Default >>nowrap and maxwidth in children = width */
/* flex-direction+flex-wrap=flex-flow */
flex-flow: row wrap;
}

.flex-children {
background-color: orangered;
width: 150px;
/* aspect-ratio: 2; */
}

.child-1 {
flex-grow: 1;
}

.child-2 {
flex-grow: 1;
}

.child-3 {
height: 200px;
aspect-ratio: 1;
}

/*
.order-1 {
order-1;
background: blue;
} */