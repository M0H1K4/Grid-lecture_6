მაგალითი 1: მარტივი Grid
HTML

html
Copy code
<div class="grid-container">
    <div class="item1">Item 1</div>
    <div class="item2">Item 2</div>
    <div class="item3">Item 3</div>
</div>
CSS

css
Copy code
.grid-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* 3 სვეტი */
    gap: 20px; /* სივრცე */
    padding: 20px; /* Padding around the grid */
}

.item1, .item2, .item3 {
    height: 100px; /* ელემენტების სიმაღლე */
    display: flex;
    align-items: center; /* ცენტრში განლაგება */
    justify-content: center; /* ცენტრში განლაგება */
    font-size: 20px; /* ტექსტის ზომა */
    border-radius: 8px; /* გრგასული კუთხეები */
}

.item1 { background-color: #4a90e2; color: white; }
.item2 { background-color: #e94e77; color: white; }
.item3 { background-color: #4caf50; color: white; }



მაგალითი 2: Grid Area
HTML

html
Copy code
<div class="grid-container">
    <div class="header">Header</div>
    <div class="sidebar">Sidebar</div>
    <div class="main">Main Content</div>
    <div class="footer">Footer</div>
</div>
CSS

css
Copy code
.grid-container {
    display: grid;
    grid-template-areas: 
        "header header"
        "sidebar main"
        "footer footer";
    grid-template-columns: 200px 1fr;
    grid-template-rows: auto 1fr auto;
    gap: 10px; /* სივრცე */
    padding: 20px; /* Padding around the grid */
}

.header, .sidebar, .main, .footer {
    padding: 20px; /* Inner padding */
    color: white; /* ტექსტის ფერი */
    border-radius: 8px; /* გრგასული კუთხეები */
}

.header { grid-area: header; background-color: #4a90e2; }
.sidebar { grid-area: sidebar; background-color: #e94e77; }
.main { grid-area: main; background-color: #4caf50; }
.footer { grid-area: footer; background-color: #f39c12; }
მაგალითი 3: Responsive Grid
HTML

html
Copy code
<div class="responsive-grid">
    <div class="item">1</div>
    <div class="item">2</div>
    <div class="item">3</div>
    <div class="item">4</div>
    <div class="item">5</div>
</div>


CSS

css
Copy code


.responsive-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Responsive სვეტები */
    gap: 15px; /* სივრცე */
    padding: 20px; /* Padding around the grid */
}

.item {
    background-color: #7ed321; /* Example color */
    padding: 40px; /* Inner padding */
    text-align: center; /* Center the text */
    border-radius: 8px; /* Rounded corners */
    font-size: 24px; /* Larger font size */
    color: white; /* Text color */
}





მაგალითი 4: Grid Item-ის განსაზღვრა
HTML

html
Copy code
<div class="grid-container">
    <div class="item-a">A</div>
    <div class="item-b">B</div>
    <div class="item-c">C</div>
</div>
CSS

css
Copy code
.grid-container {
    display: grid;
    grid-template-columns: 100px 100px;
    gap: 10px; /* Space between items */
    padding: 20px; /* Padding around the grid */
}

.item-a, .item-b, .item-c {
    background-color: #f39c12; /* Example color */
    padding: 40px; /* Inner padding */
    text-align: center; /* Center text */
    border-radius: 8px; /* Rounded corners */
    color: white; /* Text color */
    font-size: 24px; /* Larger font size */
}

.item-a {
    grid-column: 1 / 3; /* Spread across both columns */
}
დასკვნა
ამ ცვლილებების მეშვეობით თითოეული მაგალითი უფრო ლამაზად და მოსახერხებლად გამოიყურება. თუ კიდევ რაიმე კონკრეტული ცვლილება გსურთ, მოგვწერეთ!

