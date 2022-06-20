<template>
    <div class="about">
        <div class="about__container">

            <div class="about__text">
                <div class="text__container">
                  <div class="text__title"> Кто я?</div>
                  <hr class="text__hr">
                  <div class="text__paragraph">
                    <p class="text__text"> 
                      Привет! Я начинающий FullStack Web разработчик. Я только-только начинаю постигать просторы фриланса и набирать опыт. 
                    </p>
                    <br>
                    <p class="text__text">
                      Готов выполнить твою задачу <span> совершенно бесплатно </span>. Но, предупреждаю сразу: с тебя - отзыв! 
                    </p>
                    <br>
                    <p class="text__text">
                      Объективная критика приветствуется.
                    </p>
                      

                    
                  </div>
                  
                </div>
            </div>

            <div class="about__list">

            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.about {
    height: 800px;
		// .about__container

		&__container {
            
            height: 800px;
            display: flex;
            
            
		}

		// .about__text

		&__text {
            margin: 50px;
            width: 50%;
            height: 85%;
            
            
            background: #292929;
            border-radius: 50px;
            // background: #444444;
            box-shadow:  16px 16px 37px #bbbbbb, -16px -16px 37px #ffffff;

            @media(max-width: 950px) {
                margin: 0px auto;
                width: 85%;
                height: 85%;
            }


    
            
		}

	

		
}

.text {

  &__title {
    color: white;
    font-size: 80px;
    font-weight: bold;
    padding: 30px 0px 20px 45px;

    @media(max-width: 450px) {
      font-size: 60px;
    }

  
  }

  &__hr {
    border: 2px solid white;
    margin: 0px 30px;
  }

  &__paragraph {
    padding: 30px 40px;
  }

  &__text {
    font-size: 34px;
    color: rgb(240, 240, 240);
    & span{
      color:rgb(255, 255, 255);
      text-decoration: underline;

      &:hover {
        color: #8ab9ff;
      }

    }

    @media(max-width: 1300px) {
      font-size: 32px;
    }

    @media(max-width: 1100px) {
      font-size: 30px;
    }

    @media(max-width: 950px) {
      font-size: 34px;
    }

    @media(max-width: 900px) {
      font-size: 34px;
    }

    @media(max-width: 770px) {
      font-size: 32px;
    }

    @media(max-width: 650px) {
      font-size: 30px;
    }

    @media(max-width: 450px) {
      font-size: 22px;
    }

    @media(max-width: 350px) {
      font-size: 20px;
    }

  }


}


</style>