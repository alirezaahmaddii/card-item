<template>
  <section class=" card-page  ">
    <div class="container mt-5">
      <div class="items-card">
        <h1 class="mb-5 text-center">What Dashcore template offers</h1>

        <div class="row row-cols-1 row-cols-md-2">
          <div class="col mb-4" v-for="items in carditem">
            <div class="card " :class="items.background">
              <div class="card-body">
                <h5 class="card-title">{{ items.title }}</h5>
                <p class="card-text">{{ items.text }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  data: () => ({
    carditem: [
      {
        background: 'background1',
        title: 'save time',
        text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error eveniet nihil perspiciatis quia quidem quod ratione sapiente sint?'
      },
      {
        background: 'background2',
        title: 'Get things done',
        text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error eveniet nihil perspiciatis quia quidem quod ratione sapiente sint?'
      },
      {
        background: 'background3',
        title: 'Grow your business',
        text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error eveniet nihil perspiciatis quia quidem quod ratione sapiente sint?'
      },
      {
        background: 'background4',
        title: 'Accomplish your goals',
        text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error eveniet nihil perspiciatis quia quidem quod ratione sapiente sint?'
      }
    ],
  }),

}
</script>
<style lang="scss">
*, *:before, *:after {
  box-sizing: inherit;
  margin: 0;
  padding: 0;
  border: 0 none;
  position: relative;
}
.card-page {
  background-color: #F7FAFC;
  padding-top: 5px;
  padding-bottom: 45px;
  margin-top: 13rem;

  .items-card {

    .card-body {
      padding: 2rem 6rem;
    }

    .card {
      border-radius: 11px;
      box-shadow: 0px 1px 3px #d4d4d4;
      transition: 0.3s all ease-in-out;

      &:hover {
        transform: translateY(-10px);
        background-position: 0px -20px;
      }
    }

    .background1 {
      background-image: url("/media/svg/pig.svg");
      background-repeat: no-repeat;
    }

    .background2 {
      background-image: url("/media/svg/medal.svg");
      background-repeat: no-repeat;
    }

    .background3 {
      background-image: url("/media/svg/user.svg");
      background-repeat: no-repeat;
    }

    .background4 {
      background-image: url("/media/svg/laptop.svg");
      background-repeat: no-repeat;
    }
  }
}

</style>
