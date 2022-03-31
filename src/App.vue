<template>
  <div id="nav">
    <MDBNavbar expand="lg" dark bg="dark" position="top" container>
      <MDBNavbarBrand class="nav-text"
        ><i class="fab fa-pagelines"></i> Haniah</MDBNavbarBrand
      >
      <!-- Toggle button -->
      <MDBNavbarToggler
        target="#navbarRightAlignExample"
        @click="collapse5 = !collapse5"
      ></MDBNavbarToggler>
      <!-- Collapsible wrapper -->
      <MDBCollapse v-model="collapse5" id="navbarRightAlignExample">
        <MDBNavbarNav right class="mb-2 mb-lg-0">
          <!-- Right links -->
          <MDBNavbarItem router-link to="/"> Home </MDBNavbarItem>
          <MDBNavbarItem router-link :to="{ name: 'About' }">
            About
          </MDBNavbarItem>
          <MDBNavbarItem router-link :to="{ name: 'Projects' }">
            Projects</MDBNavbarItem
          >
          <MDBNavbarItem router-link :to="{ name: 'Testimonials' }">
            Testimonials</MDBNavbarItem
          >
          <MDBNavbarItem router-link :to="{ name: 'Resume' }">
            Resume
          </MDBNavbarItem>

          <MDBNavbarItem router-link :to="{ name: 'Contact' }">
            Contact
          </MDBNavbarItem>
          <!-- Right links -->
        </MDBNavbarNav>
      </MDBCollapse>
      <!-- Collapsible wrapper -->
    </MDBNavbar>
  </div>
  <router-view />
</template>

<script>
import {
  MDBNavbar,
  MDBNavbarToggler,
  MDBNavbarBrand,
  MDBNavbarNav,
  MDBNavbarItem,
  MDBCollapse,
} from "mdb-vue-ui-kit";
import { ref } from "vue";
export default {
  components: {
    MDBNavbar,
    MDBNavbarToggler,
    MDBNavbarBrand,
    MDBNavbarNav,
    MDBNavbarItem,
    MDBCollapse,
  },
  setup() {
    const collapse5 = ref(false);
    return {
      collapse5,
    };
  },

  methods: {
    handleSubmit() {
      console.log(this.name, this.mail, this.msg);
      fetch("http://localhost:5000/contact", {
        method: "POST",
        body: JSON.stringify({
          name: this.name,
          mail: this.mail,
          contact: this.contact,
          msg: this.msg,
        }),
        headers: {
          "Content-type": "application/json; charset=UTF-8",
        },
      })
        .then((response) => response.json())
        .then((json) => console.log(json))
        .catch((e) => alert(e.msg));
    },
  },
};
</script>

<style>
#app {
  font-family: sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: rgb(255, 255, 255);
}

#nav {
  padding: 10px;
}

#nav a {
  color: #fff;
  font-family: sans-serif;
}

#nav a.router-link-exact-active {
  color: rgb(216, 101, 120);
}
.nav-text {
  font-family: sans-serif;
  font-size: 30px;
  font-weight: bold;
  margin-left: 40px;
}
.fab {
  margin-bottom: 5px;
  padding-right: 8px;
  color: rgb(216, 101, 120);
}
</style>
