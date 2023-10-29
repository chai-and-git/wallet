<template>
  <div class="cards">
    <div>
      <div class="balance-text">Account Balance</div>
      <div class="details-actions">
        <div class="currency-tab">S$</div>
        <div class="amount">{{ balance }}</div>
        <div class="add-card">
          <img class="plus" src="/images/add-card.png" />
          <span>Add card</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      balance: 3000
    }
  }
}
</script>

<style lang="scss" scoped>
.cards {
  top: 45px;
  padding: 4%;
  box-sizing: border-box;
  position: relative;
  min-height: 80vw;
  background-color: #0C365A;
  color: white;

  .balance-text {
    font-size: 14pt;
    margin-bottom: 25px;
  }

  .details-actions {
    display: block;
    height: 33pt;
    box-sizing: border-box;

    .currency-tab, .amount {
      float: left;
    }

    .currency-tab {
      border-radius: 4px;
      background-color: #01D167;
      padding: 4px 5px;
      min-width: 40px;
      text-align: center;
      font-size: 12pt;
      margin-bottom: 0;
    }

    .amount {
      margin-left: 10px;
      font-size: 20pt;
    }

    .add-card {
      float: right;
      display: flex;
      flex-direction: row;
      position:relative;
      vertical-align: middle;

      .plus {
        height: 16pt;
        bottom: 6px;
      }

      span {
        margin-left: 7px;
        font-size: 13pt;
      }
    }
  }
}
</style>