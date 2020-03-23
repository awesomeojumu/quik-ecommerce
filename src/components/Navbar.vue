<template>
    <nav class="mx-auto navbar navbar-expand-lg navbar-light bg-dark">
        <b-navbar variant="faded" type="light">
            <b-navbar-brand href="#">
              <img src="https://cdn.freebiesupply.com/logos/thumbs/2x/quik-logo.png" height="50px" width="120px" class="d-inline-block align-top" alt="Kitten">
            </b-navbar-brand>
        </b-navbar>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <form class="form-inline my-1 my-md-0">
            <input class="inputsize form-control mr-lg-1" style="width: 600px; margin-left:100px;" type="search" placeholder="Search products, brands and categories" aria-label="Search products, brands and categories">
            <button class="btn btn-outline-info my-1 my-sm-0" type="submit">Search</button>
          </form>
          <ul class="navbar-nav mr-auto">
            <li class="nav-item active">
              <a class="nav-link text-primary" href="#">Home <span class="sr-only">(current)</span></a>
            </li>
            <li class="nav-item active">
              <a class="nav-link text-primary" href="#">Store</a>
            </li>
            <li class="nav-item active">
              <a class="nav-link text-primary" href="#"> Cart </a>
            </li>
            <li class="nav-item active">
              <a class="nav-link text-primary" href="#" >Help</a>
            </li>
          </ul>
        </div>
      </nav>
</template>

<script>
export default {
    name: 'Navbar'
}
</script>