<template>
    <div class="about">
        <div class="about__container">

            <div class="about__text">
                <div class="text__container">
                  <div class="text__title"> Кто я?</div>
                  <hr class="text__hr">
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
  }

  &__hr {
    border: 2px solid white;
    margin: 0px 30px;
  }

}


</style>