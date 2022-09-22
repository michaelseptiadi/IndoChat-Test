<script setup></script>

<template>
  <div class="get-touch" id="register">
    <div class="title">
      <img src="../assets/clipboard.png" alt="Clipboard" class="logo" />
      <h3>Get in touch</h3>
      <p>
        Want to get in touch? We'd love to hear from you. Here's how you can
        reach us .
      </p>
    </div>
    <div class="search-bar">
      <input type="text" placeholder="Search" class="search" />
    </div>
    <div class="form-touch">
      <div class="map">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3966.6209675178725!2d106.8220042501495!3d-6.181458095502909!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e69f42c022144c3%3A0xfe6941ee5d3ab9d8!2sWisma%20Antara%2C%20Jl.%20Medan%20Merdeka%20Sel.%20No.17%2C%20RT.11%2FRW.2%2C%20Gambir%2C%20Central%20Jakarta%20City%2C%20Jakarta%2010110!5e0!3m2!1sen!2sid!4v1663852441553!5m2!1sen!2sid"
          width="330"
          height="350"
          style="border: 0"
          allowfullscreen=""
          loading="lazy"
        ></iframe>
      </div>
      <div class="form">
        <h3>Feedback</h3>
        <form>
          <div class="fullname">
            <input type="text" placeholder="First" />
            <input type="text" placeholder="Last" />
          </div>
          <input type="text" placeholder="Email" class="input-form" />
          <textarea placeholder="Message" class="input-form" />
          <button>Send</button>
        </form>
      </div>
    </div>
  </div>
</template>

<style>
.get-touch {
  background-color: rgb(239, 239, 239);
  height: 400px;
  padding: 48px 0;
  height: fit-content;
}

.get-touch,
.title {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.title p {
  letter-spacing: 0.1em;
}

h3 {
  margin: 24px 0 12px;
}

.search-bar {
  margin: 24px 0;
}

.search {
  height: 36px;
  width: 600px;
  background-image: url("../assets/search.svg");
  background-size: 24px;
  background-position-x: 24px;
  background-position-y: center;
  background-repeat: no-repeat;
  padding: 12px 20px 12px 60px;
  border: none;
  border-radius: 12px;
}

.search:focus {
  border: none;
}

.form-touch {
  display: flex;
  justify-content: center;
  border-radius: 12px;
}

.form {
  width: 330px;
  height: 350px;
  background-color: #fff;
  padding: 0 0 0 24px;
}

.fullname input {
  padding: 4px;
  width: 140px;
  height: 24px;
  margin-right: 4px;
}

.input-form {
  margin-top: 12px;
  width: 296px;
  height: 24px;
  padding: 4px;
}

textarea {
  height: 120px !important;
}

.input-form,
.fullname input {
  border: 0.5px solid #000;
  border-radius: 8px;
  font-size: 16px;
}

@media only screen and (max-width: 950px) {
  iframe,
  .form {
    width: 250px;
    height: 300px;
  }
  .fullname input {
    margin-top: 10px;
  }
  .title p {
    letter-spacing: 0;
  }
  .search {
    width: 450px;
  }
  .input-form,
  .fullname input {
    width: 200px;
    height: 16px;
    font-size: 14px;
    padding-left: 8px;
  }
  textarea {
    height: 50px !important;
  }
}
@media only screen and (max-width: 480px) {
  .get-touch {
    width: 125%;
  }
  iframe,
  .form {
    width: 175px;
    height: 300px;
  }
  .fullname input {
    margin-top: 10px;
  }
  .title p {
    font-size: 12px;
  }
  .search {
    width: 300px;
    height: 24px;
  }
  .input-form,
  .fullname input {
    width: 140px;
    height: 16px;
    font-size: 14px;
    padding-left: 8px;
  }
  textarea {
    height: 50px !important;
  }
}
</style>
