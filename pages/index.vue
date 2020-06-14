<template>
  <el-container>
    <el-header>
      <el-menu :default-active="activeIndex" class="page-component__scroll el-scrollbar el-menu-demo" mode="horizontal" @select="handleSelect">
          <el-menu-item index="1">
            <i class="el-icon-thumb"></i>
            <a href="#nomination">How to nominate ?</a>
          </el-menu-item>
          <el-menu-item index="2">
            <i class="el-icon-user-solid"></i>
            <a href="#people">People</a>
          </el-menu-item>
          <el-menu-item index="3">
            <i class="el-icon-user-solid"></i>
            <a href="#infrastructure">Infrastructure</a>
          </el-menu-item>
          <el-menu-item index="4">
            <i class="el-icon-info"></i>
            <a href="#faq">FAQ</a>
          </el-menu-item>
      </el-menu>
    </el-header>
    <el-main>
    <div class="el-scrollbar__wrap">

    <div>
      <h2 class="introduction">Mission</h2>
      <div>
        <p>
          We would like to support the entire Polkadot ecosystem and Web3 in general. Our infrastructure setup 
          is running in a secure and robust environment to ensure your stake keeps growing in the safest place 
          without worrying too much about it. If your project is built on Substrate and would like to have a 
          robust validator infrastructure service to support, please contact us.
        </p>
        <br/>
        <p>
          MORE COMING SOON.............
        </p>
      </div>
    </div>
    <el-divider></el-divider>

    <div class=block>
      <h2 class="nomination">How to nominate our validator on Polkadot?</h2>
      <el-timeline>
        <el-timeline-item timestamp="Step 1." placement="top" type="primary" size="large">
          <el-card>
            <h2>Go to the <a href="https://polkadot.js.org/apps/#/explorer" target="_blank">PolkadotJS explorer</a> website</h2>
            <div>
              <img src="~/assets/images/nomination/1-staking-page.jpg" width="1000" />
            <p>If you are not sure whether you are connected to the Polkadot network, check the <a href="https://polkadot.js.org/apps/#/settings" target="_blank">remote node/endpoint to connect to</a> field in the Settings page.</p>
            </div>
          </el-card>
        </el-timeline-item>
        <el-timeline-item timestamp="Step 2." placement="top" type="info" size="large">
          <el-card>
            <h2>Account actions tab</h2>
            <div>
              <img src="~/assets/images/nomination/2-account-actions.jpg" width="1000" />
            <p>In this tab, you should look like this above image if you have already configurated the stash and controller account. 
              If not, please follow <a href="https://wiki.polkadot.network/docs/en/maintain-guides-how-to-nominate-polkadot#setting-up-stash-and-controller-keys" target="_blank">this guide</a> to set that up first. Once completed, you can click "Nominate" to select a number of 
              validators your trust to let them help you to earn the staking rewards..</p>
            </div>
          </el-card>
        </el-timeline-item>
        <el-timeline-item timestamp="Step 3." placement="top" type="info" size="large">
          <el-card>
            <h2>Nominate validators</h2>
            <div>
              <img src="~/assets/images/nomination/3-nominate.jpg" width="1000" />
            <p>To nominate our validator, paste <b>13YK1sHixcvVPc6v7q1F1p7e66dgoVjcSHnfv4cFJcuKbNke</b> to the input field. Then you should
              be able to see our validator on the "candidate accounts" list box. You can simply click that and it will move to the "nominated
              accounts". Then click "Nominate".</p>
            </div>
          </el-card>
        </el-timeline-item>
                <el-timeline-item timestamp="Step 4." placement="top" type="info" size="large">
          <el-card>
            <h2>Sign and submit</h2>
            <div>
              <img src="~/assets/images/nomination/4-sign-and-submit.jpg" width="1000" />
            <p>Finally, sign and submit the transaction to make it effective.</p>
            </div>
          </el-card>
        </el-timeline-item>
                <el-timeline-item timestamp="Step 5." placement="top" type="success" size="large">
          <el-card>
            <h2>Congratulation</h2>
            <div>
              <img src="~/assets/images/nomination/5-finish.jpg" width="1100" />
            <p>You have successfully nominated for our validator. Thanks for your support!❤️</p>
            </div>
          </el-card>
        </el-timeline-item>
      </el-timeline>
    </div>

    <el-divider></el-divider>

    <div id="people">
      <h2>People</h2>
      <el-row :gutter="10">
        <el-col :xs="24" :sm="12" :md="12" :lg="12" :xl="12" :span="12" >
          <el-card :body-style="{ padding: '0px' }">
            <img src="~/assets/images/profile/anson.jpg" class="image">
            <div style="padding: 14px;">
              <span>Fabio Lima@Web3 Foundation</span>
              <div class="bottom clearfix">
                <el-link href="https://github.com/lamafab" target="_blank" icon="el-icon-s-home">Github</el-link>
                <br />
                <el-link type="info" icon="el-icon-s-custom" disabled>Riot: @fabio:web3.foundation</el-link>
              </div>
            </div>
          </el-card>
        </el-col>

          <el-col :xs="24" :sm="12" :md="12" :lg="12" :xl="12" :span="12">
          <el-card :body-style="{ padding: '0px' }">
            <img src="~/assets/images/profile/anson.jpg" class="image">
            <div style="padding: 14px;">
              <span>Anson Lau@Web3 Foundation</span>
              <div class="bottom clearfix">
                <el-link href="https://github.com/ansonla3" target="_blank" icon="el-icon-s-home">Github</el-link>
                <br />
                <el-link type="info" icon="el-icon-s-custom" disabled>Riot: @anson:web3.foundation</el-link>
              </div>
            </div>
          </el-card>
        </el-col>
      </el-row>
      </div>

      <el-divider></el-divider>

      <div class="introduction" id="infrastructure">
          <h2>Infrastructure</h2>
          <div> COMING SOON. </div>
      </div>

      <el-divider></el-divider>

      <div id="faq">
        <h2>FAQ</h2>
        <el-collapse accordion>
          <el-collapse-item name="1">
            <template slot="title">
              What is our validator address?
            </template>
            <div> 
              Polkadot: 13YK1sHixcvVPc6v7q1F1p7e66dgoVjcSHnfv4cFJcuKbNke <br/>
              Kusama: CmD9vaMYoiKe7HiFnfkftwvhKbxN9bhyjcDrfFRGbifJEG8
            </div>
          </el-collapse-item>
          <el-collapse-item title="What is the commission rate for our validator ?" name="2">
            <div>
              Polkadot: 2%  <br/>
              Kusama: 10%
            </div>
          </el-collapse-item>
          <el-collapse-item title="How can you contact us?" name="4">
            <div>
                <p>Free feel to send us a message via Riot, Telegram or Wechat. =)</p> 
                Wechat: ansonlau3 <br/>
                Riot: @fabio:web3.foundation / @anson:web3.foundation
            </div>
          </el-collapse-item>
        </el-collapse>
      </div> 
    </div>
    </el-main>

    <el-backtop  :bottom="100">
      <div
        style="{
          height: 100%;
          width: 100%;
          background-color: #f2f5f6;
          box-shadow: 0 0 6px rgba(0,0,0, .12);
          text-align: center;
          line-height: 40px;
          color: #1989fa;
        }"
      >
        UP
      </div>
    </el-backtop>

    <el-footer> Build with heart @2020</el-footer>
  </el-container>
</template>

<script>

export default {
  components: {  },

  data() {
    return {
      activeIndex: '1',
    };
  },

  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  }
}
</script>

<style>

html {
  scroll-behavior: smooth;
}

.time {
  font-size: 13px;
  color: #999;
}

.bottom {
  margin-top: 13px;
  line-height: 12px;
}

.button {
  padding: 0;
  float: right;
}

.image {
  width: 50%;
  display: block;
  margin: 0 auto;
}

.clearfix:before,
.clearfix:after {
    display: table;
    content: "";
}

.clearfix:after {
    clear: both
}


.el-carousel__item h3 {
  color: #475669;
  font-size: 18px;
  opacity: 0.75;
  line-height: 300px;
  margin: 0;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n+1) {
  background-color: #d3dce6;
}

.el-col {
  border-radius: 4px;
}
.bg-purple-dark {
  background: #99a9bf;
}
.bg-purple {
  background: #d3dce6;
}
.bg-purple-light {
  background: #e5e9f2;
}
.grid-content {
  border-radius: 4px;
  min-height: 36px;
}

.container {
  margin: 0 auto;
  /* min-height: 100vh; */
  /* display: flex; */
  justify-content: center;
  align-items: center;
  text-align: center;
}

.introduction {
  text-align: center;
}

#people {
  text-align: center;
  margin-left: auto;
  margin-right: auto;
  width: 60%;
}

#faq {
  text-align: center;
  margin-left: auto;
  margin-right: auto;
  width: 60%;
}

.nomination {
  text-align: center;
}

.body {
  font-family: 'Nixie One', cursive;
}

.el-timeline {
  width: 70%;
  margin-left: auto;
  margin-right: auto;
}

.title {
  font-family: 'Nixie One', cursive;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
