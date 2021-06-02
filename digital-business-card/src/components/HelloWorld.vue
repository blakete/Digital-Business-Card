<template>
  <div>
    <v-img :src="require('@/assets/blake.jpg')"></v-img>
    <div class="business-card-body">
      <div class="name-row">
        <div class="name">Blake</div>
        <v-icon color="primary" size="24"> mdi-check-decagram </v-icon>
      </div>
      <div class="current-title">
        CEO / Founder of Alpha Wellness<br />
        Software Engineer
      </div>
      <div class="top-action-btns">
        <v-btn elevation="10" class="action-btn" style="margin-right: 17px">
          Add Contact
        </v-btn>
        <v-btn elevation="10" class="action-btn"> Connect </v-btn>
      </div>
      <div class="masonry">
        <div class="icon-container">
          <v-img
            class="icon-img"
            v-ripple
            contain
            width="118px"
            height="118px"
            :src="require('@/assets/linkedin.png')"
          >
          </v-img>
          <div class="icon-text">Connect</div>
        </div>
        <div class="icon-container">
          <v-img
            class="icon-img"
            v-ripple
            contain
            width="118px"
            height="118px"
            :src="require('@/assets/mailicon.png')"
          >
          </v-img>
          <div class="icon-text">Email</div>
        </div>
        <div class="icon-container">
          <v-img
            class="icon-img"
            v-ripple
            contain
            width="118px"
            height="118px"
            :src="require('@/assets/imessage.png')"
          >
          </v-img>
          <div class="icon-text">Text</div>
        </div>
        <div class="icon-container">
          <v-img
            class="icon-img"
            v-ripple
            contain
            width="118px"
            height="118px"
            :src="require('@/assets/contacts.png')"
          >
          </v-img>
          <div class="icon-text">Contact</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
};
</script>

<style scoped>
.business-card-body {
  position: absolute;
  top: 270px;
  left: 0px;
  background-color: white;
  width: 100%;
  padding: 15px;
}

.name-row {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-content: center;
}
.name {
  font-size: 28px;
  font-family: "proxima-nova", Arial, Helvetica, sans-serif;
  font-weight: bold;
  margin-right: 5px;
}

.current-title {
  margin-top: 14px;
  text-align: center;
  font-size: 16px;
  font-family: "proxima-nova", Arial, Helvetica, sans-serif;
}

.top-action-btns {
  margin-top: 20px;
  display: flex;
  flex-direction: row;
  align-content: center;
  justify-content: center;
}

.action-btn {
  width: 130px;
  border-radius: 7px !important;
}

.masonry {
  margin-top: 28px;
  display: flex;
  flex-flow: row wrap;
  width: 100%;
  align-content: center;
  justify-content: center;
}

.icon-container {
  margin-right: 22px;
  margin-left: 22px;
  margin-bottom: 18px;
  display: flex;
  flex-direction: column;
}

.icon-text {
  text-align: center;
}

.icon-img {
  border-radius: 25px;
}
</style>
