<template>
  <div>
    <img class="background" src="@/assets/img/background-black.svg" />
    <div></div>
    <div class="container">
      <div class="main">
        <h5 class="title">João Vale</h5>
        <h3 class="sub-title">Junior Software Developer</h3>
        <a
          class="btn"
          href="mailto:joaofilipevale@outlook.pt"
          subject="subject text"
          target="__blank"
          title="João Vale e-mail"
          >Message Me</a
        >
      </div>
      <div class="footer">
        <li class="links">
          <ul>
            <a
              class="link"
              href="https://media-exp1.licdn.com/dms/document/C4E2DAQEURhgTQTV2wA/profile-treasury-document-pdf-analyzed/0/1645128792873?e=1660176000&v=beta&t=6VHyasAGZMb5pBwngOk1oa7o8a9hEcWix18kLTbrxgA"
              target="__blank"
              title="João Vale Resume"
              >Resume</a
            >
          </ul>
          <ul>
            <a
              class="link"
              href="https://pt.linkedin.com/in/joaofilipevale"
              target="__blank"
              title="João Vale LinkedIn"
              >LinkedIn</a
            >
          </ul>
          <ul>
            <a
              class="link"
              href="https://github.com/joaofilipevale"
              target="__blank"
              title="João Vale GitHub"
              >Github</a
            >
          </ul>
        </li>
        <div class="copyright">© {{new Date().getFullYear()}} - João Vale</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainPage",
  components: {},
};
</script>

<style scoped>
.background {
  width: 100%;
  height: 100%;
  position: absolute;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
.container {
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  position: relative;
  max-width: 1480px;
  height: 100vh;
  margin: 0px auto;
  padding: 0px 20px 0px 20px;
}
.main {
  max-width: 678px;
  width: 100%;
  margin: 0 auto;
  padding-top: 8%;
  display: flex;
  flex-direction: column;
  text-align: center;
  align-items: center;
}
.title {
  font-size: 72px;
  font-weight: 700;
  line-height: 91px;
}
.sub-title {
  font-size: 36px;
  font-weight: 400;
  line-height: 45px;
  padding-top: 10px;
}
.btn {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 120px;
  height: 40px;
  background-color: #ff8e00;
  border-radius: 8px;
  color: #fff;
  font-size: 14px;
  margin: 48px auto 0px;
}
.btn:hover {
  opacity: 0.8;
  transition: 0.5s;
}
.footer {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  margin-bottom: 30px;
  max-height: 200px;
  height: 100%;
}
.links {
  display: flex;
  margin: auto;
  max-width: 536px;
  width: 100%;
  justify-content: space-between;
  font-size: 14px;
  line-height: 18px;
  font-weight: 400;
}
.link:hover {
  transition: 0s;
  font-weight: 700;
}
.copyright {
  font-size: 10px;
  margin: auto;
  margin: 0 auto;
}
@media (max-width: 707px) {
  .main {
    padding-top: 50px;
  }
}
@media (max-width: 555px) {
  .main {
    padding-top: 150px;
  }
  .title {
    line-height: 70px;
  }
  .title {
    font-size: 65px;
    line-height: 60px;
  }
  .sub-title {
    font-size: 26px;
  }
  .btn {
    margin: 40px auto 70px;
  }
}
@media (max-width: 480px) {
  .title {
    font-size: 45px;
    line-height: 40px;
  }
  .btn {
    margin-bottom: 40px;
  }
  .links {
    flex-direction: column;
    align-items: center;
    gap: 15px;
  }
  .copyright {
    font-size: 8px;
    margin-top: 25px;
  }
}
</style>