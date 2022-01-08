# Bootstrap 5 Tutorial

- prerequisities: HTML, CSS

### BS4 vs BS5

- support IE 10 and 11
- more colors added in bootstrap 5
- card-deck class is not supported anymore
- jumbotron not supported in bs5
- jQuery is removed and vanila js has taken place in bs5
- bootstrap 5 has own SVG icons
- form elements such as buttons, checkboxes used to look - different based on OS and browser now it remains same
- breakpoints: now 6 break-points xs, sm, md, lg, xl, xxl

- <div class="row bg-primary gx-3 gy-4 g-4"> </div>

### [0. welcome to Bootstrap4 and 5](https://youtu.be/Wl6Q472fNCc)

### [1. Introduction to Bootstrap](https://youtu.be/SzaWRb-Mm_M)

#### 1.1 What is Bootstrap?

- Most powerful and popular Front end framework.

#### 1.2 Why Bootstrap?

- It includes HTML, CSS based design for buttons, navigation etc.
- Easier web development
  - create navbar, alert boxes, different layout so easily
- Create responsive web page easily
- save time
- open source

### [2. Create a bootstrap webpage](https://youtu.be/B7z7_LOCvrs)

- create a basic html file with 6 heading tags
- How to add bootstrap to your project?
  - add css cdn to the head of html file : `<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous"> `
  - add js cdn inside the body: ` <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>`

### [3. Containers and grid](https://youtu.be/JVGWXp5uw7o)

- breakpoints: xs < 576px | sm >=576px | md >=768px | lg >=992 | xl >=1200px | xxl >=1400px
- .container: for x-small it will take 100%; but for other breakpoints it will take maximum not full width of viewport
- .container-fluid
- .container-{breakpoint}; example- .container-md
- example

  ```html
  <div class="container">
    <h1>Anisul Islam</h1>
    <p>Born To Teach.</p>

    <h2>About Me</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta,
      repudiandae laboriosam? Odit repudiandae beatae eius modi sapiente eveniet
      exercitationem illum.
    </p>
  </div>
  ```

- built with flexbox layout
- .row
- .col, .col-{breakpoints}; breakpoints are: xs, sm, md, lg, xl, xxl
- responsive grid
- example:
  ````html
  <div class="row">
    <h2>My Services</h2>
    <div class="col-md-4 col-md-6">
      <h3>Web development</h3>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
    </div>
    <div class="col-md-4 col-md-6">
      <h3>Web development</h3>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
    </div>
    <div class="col-md-4 col-md-6">
      <h3>Web development</h3>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
    </div>
  </div>
  ```html
  ````

### [4. bootstrap 4 vs bootstrap5](https://youtu.be/dMU3R1dWqo4)

### [5. colors and spacing - Margin, padding](https://youtu.be/OpxU0T_Pa4w)

- colors: primary(blue), success(green), info(light blue), warning(orange), danger(red), secondary(grey), white, dark, light
- bg-colorName
- text-colorName
- p-0 (no padding), p-1(0.25rem), p-2(0.5rem), p-3(1rem), p-4(1.5rem) to p-5
- pl-value; pr-value, pt-value; pb-value; px-value; py-value;
- responsive padding: p-3, p-lg-5
- use m for margin

### [6. border and image](https://youtu.be/oPlPz2gf5OY)

- border, border-colorName, rounded-left, rounded-circle
- responsive image: img-fluid
- thumbnail image: img-thumbnail
- aligning-image: float start, float-end
- centering image: mx-auto d-block or make the parent div text-center

### [7. Text and font](https://youtu.be/AbhMm6TYNKg)

- text-left, text-right, text-center, text-justify
- responsive text-alignment: text-sm-left text-md-center
- text-lowercase, text-uppercase, text-capitalize
- text-decoration-none

### [8. dismissible alert](https://youtu.be/jJnr3kvxmgU)

- example
  ```html
  <div class="alert alert-danger alert-dismissible" role="alert">
    <button
      class="btn-close"
      data-bs-dismiss="alert"
      aria-label="Close"
    ></button>
    Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sapiente, fuga!
  </div>
  ```

### [9. blockquote and abbreviations](https://youtu.be/GggXq0Dh-Jc)

- example

  ```html

  ```

### [10. button, button group, list group](https://youtu.be/rU9glyS3J6o)

- btn, btn-link, btn-group
- btn-colorName; example: btn-primary, btn-light
- btn-outline-colorName
- button modifiers: btn-lg, btn-sm, btn-block, btn-group-lg, disabled
- example

  ```html

  ```

### [11. collapse and pagination](https://youtu.be/pKrfwnZ2Rxk)

- example

  ```html
  <!-- collapse example -->
  <a href="#demo" data-bs-toggle="collapse">learn more</a>
  <button
    class="btn btn-primary"
    type="button"
    data-bs-toggle="collapse"
    data-bs-target="#demo"
    aria-expanded="false"
    aria-controls="demo"
  >
    learn more
  </button>
  <div class="collapse" id="demo">
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Id dolorem sed
      quisquam repudiandae sequi voluptatibus, aperiam aliquam adipisci nam
      maiores quia unde necessitatibus veritatis eligendi in laboriosam, officia
      porro? Explicabo.
    </p>
  </div>

  <!-- pagination example -->
  <footer>
    <ul class="pagination py-3 justify-content-center">
      <li class="page-item"><a class="page-link" href="#">1</a></li>
      <li class="page-item"><a class="page-link" href="#">2</a></li>
      <li class="page-item"><a class="page-link" href="#">3</a></li>
    </ul>
  </footer>
  ```

### [12. Navigation menu](https://youtu.be/ZbAvtMpEzcA)

- example

  ```html
  <!-- nav example -->
  <ul class="nav justify-content-center py-3 bg-primary">
    <li class="nav-item">
      <a class="nav-link text-white text-uppercase active" href="#">Home</a>
    </li>
    <li class="nav-item">
      <a class="nav-link text-white text-uppercase" href="#">Tutorial</a>
    </li>
    <li class="nav-item">
      <a class="nav-link text-white text-uppercase" href="#">Gallery</a>
    </li>
    <li class="nav-item">
      <a class="nav-link text-white text-uppercase" href="#">Contact</a>
    </li>
  </ul>
  ```

### [13. Toggleable dynamic tab and pill](https://youtu.be/VWxSH4zjF8c)

### [14. Navbar](https://youtu.be/Exq0vXXe3DM)

### [15. Card](https://youtu.be/hXNglSpEv5Q)

- example

```html
<div class="row">
  <div class="col-lg-3">
    <div class="card">
      <img
        src="http://www.studywithanis.com/wp-content/uploads/2018/01/ICT-Cover.jpg"
        alt="hsc ict"
      />
      <div class="card-body">
        <h4 class="card-title">Card Title</h4>
        <p class="card-text">card text is here. add your description</p>
        <a href="#" class="card-link stretched-link" target="_blank"
          >visit the link</a
        >
      </div>
    </div>
  </div>
</div>
```

### [16. Media objects](https://youtu.be/cqEvL_kIbTE)

### [17. Table](https://youtu.be/74Ge1I0FzBk)

- we can use table-colorName on table, tr, td
- Use .table-striped to add zebra-striping to any table row within the <tbody>.
- example

```html
          <table class="table table-bordered table-hover text-center table-striped">
        <caption>
          My Education
        </caption>
        <thead style="background-color: darkseagreen">
          <tr>
            <th scope="col">Qualification</th>
            <th scope="col">Institution</th>
            <th scope="col">Passing Year</th>
            <th scope="col">Grade</th>
          </tr>
        </thead>
        <tbody>
          <tr class="table-primary">
            <th scope="row">SSC</th>
            <td>SingerKatch High School and College</td>
            <td>2006</td>
            <td rowspan="2">3.44 / 5.00</td>
          </tr>
          <tr class="table-secondary">
            <th scope="row">HSC</td>
            <td>SingerKatch High School and College</td>
            <td>2008</td>
          </tr>
          <tr>
            <th scope="row">BSc in CSE</td>
            <td>Leading University</td>
            <td>2017</td>
            <td>3.92 / 4.00</td>
          </tr>
        </tbody>
      </table>
```

### [18. Form ](https://youtu.be/eDE7TndaKeM)

- form controls create block level and allows us to style input and textarea with custom sizing, designing and more.
- sizing: form-control, form-control-lg, form-control-sm

- example

```html
     <div id="contact-me" class="p-3">
      <h2 class="text-center">Contact</h2>
      <form action="">

        <!-- name here  -->
       <div class="mb-3">
          <label for="fullname" class="form-label">fullname: </label>
          <input type="text" id="fullname" name="fullname" class="form-control">
       </div>

       <!-- email here  -->
        <div class="mb-3">
          <label for="email" class="form-label">email: </label>
          <input type="email" id="email" name="email" class="form-control">
          <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
        </div>

        <!-- password here  -->
        <div class="mb-3">
          <label for="password" class="form-label">password: </label>
          <input type="password" id="password" name="password" class="form-control">
          <div id="passwordHelp" class="form-text">Must be 8-20 characters long.</div>
        </div>

       <!-- color selector here  -->
        <div class="mb-3">
            <label for="exampleColorInput" class="form-label">Color picker</label>
            <input type="color" class="form-control-color" id="exampleColorInput" value="#563d7c" title="Choose your color">
        </div>

        <!-- dropdown menu here  -->
        <div class="mb-3">
            <select class="form-select" aria-label="department">
               <option selected>CSE</option>
               <option value="1">EEE</option>
               <option value="2">LLB</option>
            </select>
        </div>

        <!-- checkbox here  -->
         <div class="mb-3">
          <div class="form-check">
            <input class="form-check-input" type="checkbox" id="terms">
            <label class="form-check-label" for="terms">
              Accept terms and conditions
            </label>
          </div>
        </div>


        <!-- radio button  -->
         <div class="mb-3">
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" id="male" name="gender">
            <label class="form-check-label" for="male">
              male
            </label>
          </div>
          <div class="form-check form-check-inline">
            <input class="form-check-input" type="radio" id="male" name="gender">
            <label class="form-check-label" for="female">
              female
            </label>
          </div>
        </div>


        <!-- form-floating labels example; placeholder is required  -->

            <div class="form-floating mb-3">
              <input type="email" class="form-control" id="emailInput" placeholder="name@example.com">
              <label for="emailInput">Email address</label>
            </div>

            <div class="form-floating">
              <textarea class="form-control" placeholder="Leave a comment here" id="floatingTextarea"></textarea>
              <label for="floatingTextarea">Comments</label>
            </div>
        </div>


          <!-- form grid example  -->
          <div class="row">
            <div class="col">
              <input type="text" class="form-control" placeholder="First name" aria-label="First name">
            </div>
            <div class="col">
              <input type="text" class="form-control" placeholder="Last name" aria-label="Last name">
            </div>
          </div>

          <button class="btn btn-primary" type="submit">Submit</button>
        </div>
      </form>
```

### [19. Carousel](https://youtu.be/f6nCsa6Zbjg)

### [20. Badge, progress and tooltip](https://youtu.be/D-rPnaM0agw)

- example

  ```html
  <h2>
    Bootstrap5 video <span class="badge bg-secondary rounded-pill">New</span>
  </h2>

  <button type="button" class="btn btn-primary">
    Notifications <span class="badge bg-secondary">4</span>
  </button>

  <button
    type="button"
    class="btn btn-secondary"
    data-bs-toggle="tooltip"
    data-bs-placement="right"
    title="by clicking sign up you will be registered"
  >
    sign up
  </button>

  <div class="progress mt-3">
    <div
      class="progress-bar bg-success w-75"
      role="progressbar"
      aria-valuenow="75"
      aria-valuemin="0"
      aria-valuemax="100"
    >
      75%
    </div>
  </div>
  ```

### [21. List group]()

- example

  ```html
  <!-- list can have link and button  -->
  <ul class="list-group">
    <li class="list-group-item active">An item</li>
    <a href="#" class="list-group-item list-group-item-action"
      >A second link item</a
    >
    <button type="button" class="list-group-item list-group-item-action">
      A third button item
    </button>
    <li class="list-group-item">A fourth item</li>
    <li class="list-group-item">And a fifth one</li>
  </ul>

  <!-- list, badge  -->
  <ul class="list-group">
    <li
      class="list-group-item d-flex justify-content-between align-items-center"
    >
      Books
      <span class="badge bg-primary rounded-pill">10</span>
    </li>
    <li
      class="list-group-item d-flex justify-content-between align-items-center"
    >
      Pens
      <span class="badge bg-primary rounded-pill">5</span>
    </li>
  </ul>
  ```

### [22. float and svg icons](https://youtu.be/-BP8r0vMOXU)

- bootstrap svg icons - https://icons.getbootstrap.com/
- example

  ```html
  <div class="clearfix">
    <div class="float-start w-50">
      <p>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Debitis,
        architecto, totam harum eaque commodi dignissimos alias veniam tenetur
        maxime, sapiente nisi facere ipsa saepe inventore.
      </p>
    </div>
    <div class="float-end w-50">
      <p>
        <i class="bi bi-123"></i>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Debitis,
        architecto, totam harum eaque commodi dignissimos alias veniam tenetur
        maxime, sapiente nisi facere ipsa saepe inventore.
      </p>
    </div>
  </div>

  <button class="btn btn-primary">
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="16"
      height="16"
      fill="currentColor"
      class="bi bi-alarm"
      viewBox="0 0 16 16"
    >
      <path
        d="M8.5 5.5a.5.5 0 0 0-1 0v3.362l-1.429 2.38a.5.5 0 1 0 .858.515l1.5-2.5A.5.5 0 0 0 8.5 9V5.5z"
      />
      <path
        d="M6.5 0a.5.5 0 0 0 0 1H7v1.07a7.001 7.001 0 0 0-3.273 12.474l-.602.602a.5.5 0 0 0 .707.708l.746-.746A6.97 6.97 0 0 0 8 16a6.97 6.97 0 0 0 3.422-.892l.746.746a.5.5 0 0 0 .707-.708l-.601-.602A7.001 7.001 0 0 0 9 2.07V1h.5a.5.5 0 0 0 0-1h-3zm1.038 3.018a6.093 6.093 0 0 1 .924 0 6 6 0 1 1-.924 0zM0 3.5c0 .753.333 1.429.86 1.887A8.035 8.035 0 0 1 4.387 1.86 2.5 2.5 0 0 0 0 3.5zM13.5 1c-.753 0-1.429.333-1.887.86a8.035 8.035 0 0 1 3.527 3.527A2.5 2.5 0 0 0 13.5 1z"
      />
    </svg>
    Alarm
  </button>
  ```

### [23. position and display](https://youtu.be/qknEBRJBAM0)

- example

  ```html
  <!-- // display: none, block, inline, inline-block, flex, grid, table -->

  <!-- <button class="d-none">click me 1</button>
    <button class="d-block">click me 2</button>
  
    <div class="bg-success d-inline-block">
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. A culpa</p>
    </div>
    <div class="bg-primary d-inline-block">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus
        tempore in qui. Quasi, quas non?
      </p>
    </div> -->

  <!-- positioning: static, fixed, sticky, absolute, relative -->

  <div class="bg-success position-relative" style="height: 200px">
    <button class="position-absolute start-50 top-50 translate-middle">
      click me
    </button>
  </div>
  ```

### [24. flex]()

- example

```html
<!-- responsive flex items -->
<div
  class="card-container d-flex flex-sm-column flex-md-row bg-success p-3"
  <!--
>
  <div class="card w-25">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
</div>

<!-- horizontal alignment  -->
<!-- justify-content-value; here value can be start, end, center, between, around, evenly -->
<div
  class="card-container d-flex flex-sm-column flex-md-row bg-success p-3 justify-content-evenly"
>
  <div class="card w-25">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
</div>

<!-- vertical alignment -->
<!-- align-items-value; here value can be start,end,center, stretch -->

<div
  class="card-container d-flex flex-sm-column flex-md-row bg-success p-3 align-items-center"
  style="height: 100vh"
  <!--
>
  <div class="card w-25">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
</div>

<!-- horizontal and vertical alignment together -->

<div
  class="card-container d-flex flex-sm-column flex-md-row bg-primary p-3 justify-content-center align-items-center"
  style="height: 100vh"
  <!--
>
  <div class="card w-25 m-1">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25 m-1">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25 m-1">
    <div class="card-body">
      <h4 class="card-title">card title</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
</div>

<!-- order of flex items -->
<div
  class="card-container d-flex flex-sm-column flex-md-row bg-primary p-3 justify-content-center align-items-center"
  style="height: 100vh"
  <!--
>
  <div class="card w-25 m-1 order-3">
    <div class="card-body">
      <h4 class="card-title">card title1</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25 m-1 order-1">
    <div class="card-body">
      <h4 class="card-title">card title2</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25 m-1 order-2">
    <div class="card-body">
      <h4 class="card-title">card title3</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
</div>

<!-- align-self: start / end/ center / stretched -->
<div
  class="card-container d-flex flex-sm-column flex-md-row bg-primary p-3 justify-content-center align-items-center"
  style="height: 100vh"
  <!--
>
  <div class="card w-25 m-1 align-self-start">
    <div class="card-body">
      <h4 class="card-title">card title1</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25 m-1">
    <div class="card-body">
      <h4 class="card-title">card title2</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
  <div class="card w-25 m-1 align-self-end">
    <div class="card-body">
      <h4 class="card-title">card title3</h4>
      <p class="card-text">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </div>
  </div>
</div>
```

### [25. Modal]()

- example

```html
<!-- modal example  -->
<!-- Button trigger modal -->
<button
  type="button"
  class="btn btn-primary"
  data-bs-toggle="modal"
  data-bs-target="#exampleModal"
>
  Launch demo modal
</button>

<!-- Modal -->
<div class="modal fade" id="exampleModal">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Modal title</h5>
        <button
          type="button"
          class="btn-close"
          data-bs-dismiss="modal"
          aria-label="Close"
        ></button>
      </div>
      <div class="modal-body">some text is here</div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">
          Close
        </button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </div>
    </div>
  </div>
</div>
```

### [26. Projects]()
