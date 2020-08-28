<template>
  <!--提示关注微信公众号页面-->
  <div class="needAttention" :class="{'blueThemeAttention':ThemeWxBank ===1}">
    <div class="contentView">
      <img src="../assets/logo.png" class="bankLogo">
      <div class="attentionText">
        <p class="prompt">您还未关注</p>
        <p class="prompt">黄河农村商业银行微信银行</p>
        <img src="../assets/theQR.jpg" class="theQR">
        <p class="promptUnder">长按二维码识别</p>
        <p class="promptUnder">“黄河农村商业银行微信银行”</p>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: "needAttention",
  data() {
    return {
      ThemeWxBank: 0
    }
  },
}
</script>

<style scoped lang="scss">
.needAttention {
  padding: 140px 30px 0;
  background-image: url(../assets/banner.png);
  background-size: 100% auto;
  background-repeat: no-repeat;

  .contentView {
    min-height: 895px;
    box-sizing: border-box;
    background-color: #fff;
    border-radius: 8px;
    position: relative;

    .bankLogo {
      width: 365px;
      height: auto;
      position: absolute;
      left: 50%;
      top: 0;
      transform: translate(-50%, -70px);
    }

    .attentionText {
      font-size: 28px;
      display: flex;
      flex-direction: column;
      justify-content: flex-start;
      align-items: center;
      padding-top: 230px;

      .theQR {
        width: 340px;
        height: 340px;
        margin: 40px 0 30px;
      }

      .prompt {
        color: #C52D21;
        line-height: 48px;
      }

      .promptUnder {
        color: #666;
        line-height: 48px;
      }
    }
  }
}

.blueThemeAttention {
  background-image: url(../assets/bannerBlue.png);
}
</style>
