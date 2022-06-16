<template>
    <div class="about">
        <div class="about__container">
            <div class="about__text">
                <div class="text__container">

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


</style>