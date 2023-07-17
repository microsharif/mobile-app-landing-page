<script setup>

/* Menue */
 const menueItemList = [
  '<a id="GoToHome" class="selected-nav" href="#intro">Home</a>',
  '<a id="GoToFeatures" href="#features">Features</a>',
  '<a id="GoToTestimonials" href="#testimonials-rotator">Testimonials</a>',
  '<a id="GoToFAQ" href="#faq">FAQ</a>',
  '<a id="GoToSubscribe" href="#newsletter">Subscribe</a>'
 ]

/* banner */
  const banner= {
    title: "Use Ritmo to create",
    subtitle: "the awesome App landing page",
    description: `<p>Vestibulum at est vel felis adipiscing tincidunt. Proin quis diam ac lectus pretium mollis interdum sed erat. Phasellus eget
                  neque eu ipsum laoreet suscipit tincidunt suscipit purus rutrum sagittis turpis
                </p>
              
                <p>Etiam euismod, ligula nec volutpat tempor, risus lerisque tincidunt purus libero fusce tincidunt ligula mollis</p>`,
  }

  const bannerIntroStoeSrc = [
    {src:'img/icons/appstore.png', alt:'appstore_icon'},
    {src:'img/icons/google.png', alt:'google_icon'},
    {src:'img/icons/amazon.png', alt:'amazon_icon'},
  ]

  const bannerIntroImgSrc = 'img/thumbs/intro_image.png'

  /* Feature List */
  const featureListTitle = 'What You’re Getting'

  const featureList = [
    {
      id: 'feature-1',
      title: 'Responsive Design',
      desripton: 'Lorem ipsum dolor and consectetur adipisicing incididunt eiusmod tempor incididunt laboredolore aliqua',
      iconCalss:'fa fa-paper-plane'
    },
    {
      id: 'feature-2',
      title: 'Web Marketing',
      desripton: 'Lorem ipsum dolor and consectetur adipisicing incididunt eiusmod tempor incididunt magna aliqua',
      iconCalss:'fa fa-globe'
    },
    {
      id: 'feature-3',
      title: 'Desktop Friendly',
      desripton: 'Lorem ipsum dolor and consectetur adipisicing incididunt eiusmod tempor incididunt magna',
      iconCalss:'fa fa-bomb'
    },
    {
      id: 'feature-4',
      title: 'Very easy to customize',
      desripton: 'Lorem ipsum dolor consectetur adipisicing incididunt eiusmod tempor incididunt laboredolore magna',
      iconCalss:'fa fa-cog'
    },
    {
      id: 'feature-5',
      title: 'Multi-language Interface',
      desripton: 'Lorem ipsum dolor and consectetur adipisicing incididunt eiusmod tempor incididunt magna',
      iconCalss:'fa fa-language'
    },
    {
      id: 'feature-6',
      title: 'Premium Support',
      desripton: 'Lorem ipsum dolor and consectetur adipisicing incididunt eiusmod tempor incididunt laboredolore aliqua',
      iconCalss:'fa fa-life-ring'
    },
  ]

  /* Call to Action */
  const callToActionTitle = "Try <span>Ritmo </span> yourself to see how easy it is"
  const callToActionDesc  = "Vestibulum at est vel felis adipiscing tincidunt quis pretium mollis"
  const callToActionBtnStyle = `
    background-color: #19acca;
    color: #fff;
    font-size: 18px;
    font-family: 'Raleway', sans-serif;
    font-weight: 700;
    padding: 10px 20px;
    border-radius: 0px;
    transition: all 200ms ease-in-out;
  `

  /* Feature One */
  const featureOneTitle = "Fully responsive layout"
  const featureOneDesc = `<p>Vestibulum at est vel felis adipiscing tincidunt. Proin quis diam ac lectus pretium mollis interdum sed erat. Phasellus eget
							  neque eu ipsum laoreet suscipit tincidunt suscipit purus rutrum 
							</p>

  <p>Etiam euismod, ligula nec volutpat tempor, risus lerisque tincidunt purus libero. Fusce tincidunt ligula, nec sagittis turpis</p>`

  const featureOneImgSrc = {src:"img/thumbs/feature_one_img.png", alt:"feature_one_img"}

  /* Feature Two */
  const featureTwoTitle = "Super easy to customize and well detailed for beginners"
  const featureTwoDesc = `<p>Vestibulum at est vel felis adipiscing tincidunt. Proin quis diam ac lectus pretium mollis interdum sed erat. Phasellus eget neque eu ipsum laoreet suscipit tincidunt suscipit purus rutrum </p>
  <p>Etiam euismod, ligula nec volutpat tempor, risus lerisque tincidunt purus libero. Fusce tincidunt ligula, nec sagittis turpis</p>`

  const featureTwoImgSrc = {src:"img/thumbs/feature_two_img.png", alt:"feature_two_img"}

  /* STATISTIC BANNER */
  const staticBannerItem = [
    {
      icon:`<i class="fa fa-cloud-download"></i>`,
      number: '1123',
      text:'Downloads'
    },
    {
      icon:`<i class="fa fa-trophy"></i>`,
      number: '58',
      text:'Winning Awards'
    },
    {
      icon:`<i class="fa fa-star"></i>`,
      number: '868',
      text:'People Rated 5'
    },
    {
      icon:`<i class="fa fa-twitter"></i>`,
      number: '575',
      text:'Followers'
    }
  ]

  /* Feature Three */
  const featureThreeTitle = "Clean and ultra modern design"
  const featureThreeDesc = `<p>Etiam euismod, ligula nec volutpat tempor, risus lerisque tincidunt purus libero. Fusce tincidunt ligula, nec sagittis turpis</p>
  <p>Vestibulum at est vel felis adipiscing tincidunt. Proin quis diam ac lectus pretium mollis interdum sed erat. Phasellus eget
    neque eu ipsum laoreet suscipit tincidunt suscipit purus rutrum</p>`

  const featureThreeList = [
    `<h5><i class="fa fa-check-square"></i>Vestibulum bibendum ullamcorper hend tellus</h5>`,
    `<h5><i class="fa fa-check-square"></i>Aliquam a suscipit, bibendum hendrerit tellus </h5>`,
    `<h5><i class="fa fa-check-square"></i>Aliquam rhoncus bibendum ullamcorper hendrerit </h5>`,
    `<h5><i class="fa fa-check-square"></i>Bibendum luctus neque laoreet rhoncus hendrerit</h5>`,
    `<h5><i class="fa fa-check-square"></i>Aliquam a augue suscipit hendrerit</h5>`,
  ]

  const featureThreeImgSrc = 'img/thumbs/feature_three_img.png'

  /* TESTIMONIALS ROTATOR */
  const testimonialRotatorList = [
    `<div class="client-msg">										
      <p>&laquo; Etiam condimentum sapien sem condimentum accumsan. Proin in adipiscing elit. Suspendisse dignissim sollicitudin 
          ornare at sagittis elementum vulputate congue &raquo;												   
      </p>												
    </div>
    <p class="author">Jonathan Doe <span>Programmer</span></p>`,

    `<div class="client-msg">										
      <p>&laquo; Etiam condimentum sapien sem condimentum accumsan. Proin in adipiscing elit. Suspendisse dignissim sollicitudin 
          ornare at sagittis elementum vulputate congue &raquo; Suspendisse dignissim sollicitudin 
          ornare at sagittis elementum vulputate congue												   
      </p>												
    </div>
    <p class="author">Karen Olson <span>Programmer</span></p>`,

    `<div class="client-msg">										
      <p>&laquo; Etiam condimentum sapien sem condimentum accumsan. Proin in adipiscing elit. Suspendisse dignissim sollicitudin 
          ornare at sagittis elementum vulputate congue &raquo;												   
      </p>												
    </div>
    <p class="author">Jonathan Doe <span>Programmer</span></p>`,

    `<div class="client-msg">													
      <p>&laquo; Vivamus a purus lacus tempor volutpat. Etiam odio purus, placerat interdum vestibulum rutrum aliquet vulputate.
          Proin euismod pulvinar aliquam &raquo; 
      </p>													
    </div>
    <p class="author">Hannah Brown <span>Internet Surfer</span></p>`
  ]

  /* FAQs */
  const faqsTitle = 'Have a few questions? Of course you do. We\'ve got answers!'
  const faqsList = [
    {
      id:'question_1',
      quention: 'Aliquam dapibus interdum lobortis ornare ipsum primis in faucibus orci mauris suscipit bibendum?',
      answer: 'Praesent semper, lacus sed cursus porta, odio augue feugiat eros, ac tincidunt ligula massa in est. Etiam ut mi sit amet mauris suscipit bibendum sit amet in odio. Integer congue leo metus.'
    },
    {
      id:'question_2',
      quention: 'Aliquam lobortis pretium ornare erat?',
      answer: 'Praesent semper, lacus sed cursus porta, odio augue feugiat eros, ac tincidunt ligula massa in est. Etiam ut mi sit amet mauris suscipit bibendum sit amet in odio. Integer congue leo metus.'
    },
    {
      id:'question_3',
      quention: 'Aliquam dapibus interdum turpis, lobortis pretium?',
      answer: 'Praesent semper, lacus sed cursus porta, odio augue feugiat eros, ac tincidunt ligula massa in est. Vestibulum ante ipsum primis in faucibus amet mauris suscipitbibendum. Praesent semper, lacus sed cursus porta, odio augue feugiat eros. '
    },
    {
      id:'question_4',
      quention: 'Aliquam interdum, lobortis pretium ornare erat?',
      answer: 'Praesent semper, lacus sed cursus porta, odio augue feugiat eros. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere suscipit bibendum sit amet in odio. Integer congue leo metus, mollis lorem viverra.'
    },
    {
      id:'question_5',
      quention: 'Aliquam dapibus interdum turpis, lobortis?',
      answer: 'Praesent semper, lacus sed cursus porta, odio augue feugiat eros, ac tincidunt ligula massa in est. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae.'
    },
    {
      id:'question_6',
      quention: 'Aliquam interdum, lobortis pretium ornare erat?',
      answer: 'Praesent semper, lacus sed cursus porta, odio augue feugiat eros. Vestibulum ante ipsum primis in faucibus orci luctus et  ultrices posuere cubilia Curae; Integer congue leo metus, mollis lorem viverra.'
    },
  ]

  /* NEWSLETTER */
  const newsLaterTitle = "Sign up for our newsletter now"
  const newsLaterSubtitle = "Be amongst the first to know about news and upcoming features"
  const newsLaterBtnStyle = `
    width: 16%;
    background-color: #19acca;
    color: #fff;
    font-size: 18px;
    font-family: 'Raleway', sans-serif;
    font-weight: 300;
    text-transform: uppercase;
    margin-left: 10px;
    padding: 10px 15px;
    border: medium none;
    border-radius: 5px;
    transition: all 250ms ease-in-out;
  `

  /* Footer */
  const footerSocialIcon = [
  `<a class="foo_social ico-facebook" href="#"><i class="fa fa-facebook"></i></a>`,
  `<a class="foo_social ico-twitter" href="#"><i class="fa fa-twitter"></i></a>`,
  `<a class="foo_social ico-google-plus" href="#"><i class="fa fa-google-plus"></i></a>`,
  `<a class="foo_social ico-behance" href="#"><i class="fa fa-behance"></i></a>`,
  `<a class="foo_social ico-dribbble" href="#"><i class="fa fa-dribbble"></i></a>`,
  ]

</script>

<template>

  <!-- HEADER
		============================================= -->
  <header id="header">		
    <div class="navbar navbar-fixed-top">	
      <div class="container">
      
        
        <!-- Navigation Bar -->
        <div class="navbar-header">
        
          <!-- Responsive Menu -->
          <button type="button" id="nav-toggle" class="navbar-toggle" data-toggle="collapse" data-target="#navigation-menu">
            <span class="sr-only">Toggle navigation</span> 
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
          </button>
          {{ selectedMenue }}
          <!-- Logo Image -->
          <a class="navbar-brand" href="#"><img src="../public/img/logo.png" alt="logo" role="banner"></a>
          
        </div>	<!-- End Navigation Bar -->
        
        
        <!-- Navigation Menu -->
					<nav id="navigation-menu" class="collapse navbar-collapse"  role="navigation">
						<ul class="nav navbar-nav navbar-right">
							<li v-for="menuItem in menueItemList" v-html="menuItem"></li>
						</ul>
					</nav>  <!-- End Navigation Menu -->
        
        
      </div>	  <!-- End container -->
    </div>		<!-- End navbar fixed top  -->		
	</header>	<!-- END HEADER -->


    <!-- CONTENT WRAPPER
		============================================= -->
		<div id="content_wrapper">

      <!-- INTRO
			============================================= -->
			<section id="intro">
				<div class="container">
					<div class="row">
					
						<!-- Intro Description -->
						<div  id="intro_description" class="col-md-7 col-lg-6">
						
							<h1>{{ banner.title }}</h1>
							<h2>{{ banner.subtitle }}</h2>
							
              <div v-html="banner.description"></div>
						
							<!-- Store Buttons -->
							<div id="intro_stores">
								<a v-for="storeSrc in bannerIntroStoeSrc" href="#">
                  <img v-bind="storeSrc"/>
                </a>			
								<!-- <a href="#"><img src="img/icons/windows.png" alt="windows_icon" /></a> -->
							</div>
						
						</div>	<!-- End Intro Description -->
						
									
						<!-- Intro Image -->
						<div id="intro_image" class="col-md-5 col-lg-6 text-center">						
							<img class="img-responsive" :src="bannerIntroImgSrc" alt="intro_image">							
						</div><!-- End Intro Header Image -->
					

					</div>	 <!-- End row -->					
				</div>	   <!-- End container -->
			</section>	 <!-- END INTRO -->

      <!-- FEATURES LIST
			============================================= -->
			<section id="features">
				<div class="container">					
					<div class="row">
					
					
						<!-- Features Holder -->
						<div id="features_holder" class="col-md-12">					
						
							<!-- Features Holder Title -->
							<div class="features_title text-center">						
								<h1>{{ featureListTitle }}</h1>
							</div>
							
						
							<!-- Features List -->
							<ul class="features_list">
							
								<!-- Feature Icon 1 -->
								<li v-for="feature in featureList" :id="feature.id">       									
									<div class="col-sm-6 col-md-4 feature-box triggerAnimation animated clearfix" data-animate="bounceIn">	
										<div class="feature-box-icon">
											<i :class="feature.iconCalss"></i>
										</div>
													
										<div class="feature-box-content">
											<h4>{{ feature.title }}</h4>
											<p>{{ feature.desripton }}</p>
										</div>
									</div>
								</li>
									
							</ul>	<!-- End Features List -->
																	
						</div>	<!-- Features Holder -->
						
						
					</div>	<!-- End row -->					
				</div>	  <!-- End container -->
			</section>	<!-- END FEATURES LIST -->

      <!-- CALL TO ACTION
			============================================= -->
			<div id="call_to_action" class="parallax">
				<div class="container">			
					<div class="row">
					
					
						<!-- Call To Action Slogan -->
						<div id="cta_slogan" class="col-md-9">
							<h2 v-html="callToActionTitle"></h2>
							<p>{{ callToActionDesc }}</p>
						</div>
						
						
						<!-- Call To Action Button -->
						<div id="cta_button" class="col-md-3 text-right">
							<a href="#" class="btn btn-lg" :style="callToActionBtnStyle">Download Now</a>
						</div>
						
											
					</div>	<!-- End row -->				
				</div>	<!-- End container -->	
			</div>	  <!-- END CALL TO ACTION -->

      <!-- FEATURE_ONE
			============================================= -->		
			<section id="feature_one">
				<div class="container">
					<div class="row">	
					
					
						<!-- Feature One Image -->
						<div id="feature_1_image" class="col-md-7 feature_image text-center triggerAnimation animated" data-animate="fadeInLeft">
							<img class="img-responsive" v-bind="featureOneImgSrc">
						</div>
						
					
						<!-- Feature One Description -->
						<div id="feature_1_description" class="col-md-5 feature_description triggerAnimation animated" data-animate="fadeInRight">
						
							<h2>{{ featureOneTitle }}</h2>

              <div v-html="featureOneDesc"></div>
							
						</div>	<!-- Feature One Description -->
						
						
					</div>	<!-- End row -->	
					
					<hr />	<!-- Horizontal Line -->

				</div>	  <!-- End container -->
			</section>	<!-- END FEATURE_ONE -->	

      <!-- FEATURE_TWO
			============================================= -->		
			<section id="feature_two">
				<div class="container">
					<div class="row">
					
					
						<!-- Feature Two Description -->
						<div id="feature_2_description" class="col-md-5 feature_description triggerAnimation animated" data-animate="fadeInLeft">
						
							<h2>{{ featureTwoTitle }}</h2>
              <div v-html="featureTwoDesc"></div>
							
						</div>	<!-- End Feature Two Description -->
						

						<!-- Feature Two Image -->
						<div id="feature_2_image" class="col-md-7 feature_image text-right triggerAnimation animated" data-animate="fadeInRight">
							<img class="img-responsive" v-bind="featureTwoImgSrc">
						</div>
						
						
					</div>	  <!-- End row -->	
				</div>	   <!-- End container -->
			</section>	<!-- END FEATURE_TWO -->

      <!-- STATISTIC BANNER
			============================================= -->
			<div id="statistic-banner" class="parallax">
				<div class="container">	
				

					<!-- Statistic Holder -->
					<div id="statistic-holder" class="row">

						<!-- Statistic Element #1 -->
						<div v-for="statistic in staticBannerItem" class="col-xs-3 col-sm-3 col-md-3 statistic-block triggerAnimation animated" data-animate="bounceIn">
							<div class="statistic-icon" v-html="statistic.icon"></div>
							<div class="statistic-number">{{ statistic.number }}</div>
							<div class="statistic-text">{{ statistic.text }}</div>
						</div>
									
					</div>	<!-- End Statistic Holder -->
					
						
				</div>	<!-- End container -->
			</div>	  <!-- END STATISTIC BANNER -->

      <!-- FEATURE_THREE
			============================================= -->		
			<section id="feature_three">
				<div class="container">
					<div class="row">	
					
					
						<!-- Feature Three Image -->
						<div id="feature_3_image" class="col-md-6 feature_image triggerAnimation animated" data-animate="fadeInLeft">
							<img class="img-responsive" :src="featureThreeImgSrc" alt="feature_three_img">
						</div>
						
						
						<!-- Feature Three Description -->
						<div id="feature_3_description" class="col-md-6 feature_description triggerAnimation animated" data-animate="fadeInRight">
						
							<h2>{{ featureThreeTitle }}</h2>
              <div v-html="featureThreeDesc"></div>
							<!-- Feature List -->
							<div id="feature_three_list">

								<!-- List Item #1 -->
								<div class="list-item" v-for="feature in featureThreeList" v-html="feature"></div>
                
							</div>	<!-- End Feature List -->	
						
						</div>	<!-- End Feature Three Description -->
						
						
					</div>	<!-- End row -->	
					
				</div>	  <!-- End container -->
			</section>	<!-- END FEATURE_THREE -->

      <!-- TESTIMONIALS ROTATOR
			============================================= -->
			<div id="testimonials-rotator">
				<div class="container text-center">
					<div class="row">					
						<div class="col-md-12">
							<!-- Rotator Content -->
							<div class="flexslider">											
								<ul class="slides">					
									<!--Testimonial #1 -->
									<li v-for="testimonialItem in testimonialRotatorList">
										<div class="testimonials" v-html="testimonialItem"></div>
									</li>																
								</ul>												
							</div>	 <!-- End Rotator Content -->	
						</div>	<!-- End col-sm-12 -->							
					</div>	<!-- End row -->  
          <hr />	<!-- Horizontal Line -->						
				</div>	 <!-- End container -->
			</div>	   <!-- END TESTIMONIALS ROTATOR -->

      <!-- FAQs
			============================================= -->		
			<section id="faq">
				<div class="container">	
				
					
					<!-- Section Title -->	
					<div class="row">
						<div class="col-md-12 text-center">
							<h1>{{ faqsTitle }}</h1>
						</div>
					</div>
					
					
					<div class="row">
						
						<!-- Question #1-->
						<div :id="faqsList[0].id" class="col-md-6 triggerAnimation animated" data-animate="bounceIn">	
							<div class="question">
								<h4>{{ faqsList[0].quention }}</h4>
								<p>{{ faqsList[0].answer }}</p>
							</div>							
						</div>
							
						<!-- Question #2-->
						<div :id="faqsList[1].id" class="col-md-6 triggerAnimation animated" data-animate="bounceIn">							
							<div class="question">
								<h4>{{ faqsList[1].quention }}</h4>
								<p>{{ faqsList[1].answer }}</p>
							</div>
						</div>
							
					</div>	<!-- End row -->	
					
					
					<div class="row">
						
						<!-- Question #3-->
						<div :id="faqsList[2].id" class="col-md-6 triggerAnimation animated" data-animate="bounceIn">	
							<div class="question">
								<h4>{{ faqsList[2].quention }}</h4>
								<p>{{ faqsList[2].answer }}</p>
							</div>							
						</div>
							
						<!-- Question #4-->
						<div :id="faqsList[3].id" class="col-md-6 triggerAnimation animated" data-animate="bounceIn">							
							<div class="question">
								<h4>{{ faqsList[3].quention }}</h4>
								<p>{{faqsList[3].answer}}</p>
							</div>
						</div>
						
					</div>	<!-- End row -->
					
						
					<div id="last_row" class="row">
						
						<!-- Question #5-->
						<div :id="faqsList[4].id" class="col-md-6 triggerAnimation animated" data-animate="bounceIn">	
							<div class="question">
								<h4>{{ faqsList[4].quention }}</h4>
								<p>{{ faqsList[4].answer }}</p>
							</div>							
						</div>
							
						<!-- Question #6-->
						<div :id="faqsList[5].id" class="col-md-6 triggerAnimation animated" data-animate="bounceIn">							
							<div class="question">
								<h4>{{ faqsList[5].quention }}</h4>
								<p>{{ faqsList[5].answer }}</p>
							</div>
						</div>
						
					</div>	<!-- End row -->
						
				</div>	   <!-- End container -->		
			</section>  <!-- END FAQs -->

      <!-- NEWSLETTER
			============================================= -->		
			<section id="newsletter">
				<div class="container">
				
				
					<!-- Newsletter Title -->		
					<div class="row">
						<div class="col-sm-12 text-center triggerAnimation animated" data-animate="fadeInDown">
							<h1>{{ newsLaterTitle }}</h1>
							<p>{{ newsLaterSubtitle }}</p>
						</div>
					</div>
					
				
					<!-- Newsletter Form -->	
					<div class="row">
					
						<div class="col-md-12 text-center triggerAnimation animated" data-animate="fadeInUp">
						
							<!-- Newsletter Form Message -->	
							<div class="message"></div>
										
							<form id="newsletter_form" method="post" action="https://dsathemes.com/html/ritmo/light/image/newsletter.php">
								<div id="newsletterfields">
									<input id="email" type="email" value="" name="email" placeholder="Enter your email address">
									<input type="submit" value="Notify Me" :style="newsLaterBtnStyle">
								</div>
							</form>	

						</div>					
						
					</div>	<!-- End row -->
					
					
				</div>	  <!-- End container -->
			</section>	<!-- END NEWSLETTER -->

      <!-- FOOTER
			============================================= -->
			<footer id="footer">
				<div class="container">
				
				
					<!-- Footer Social Icons -->
					<div class="row">									
						<div id="footer_icons" class="col-md-12 text-center">																	
							<ul class="footer-socials clearfix">
								<li v-for="socialItem in footerSocialIcon" v-html="socialItem"></li>							
							</ul>
						</div>	 <!-- End Footer Social Icons -->	
					</div>
				
				
					<!-- Footer Copy-->
					<div class="row">	
						<div id="footer_copy" class="col-sm-12 text-center">	
							<p>Mobile App Landing Page.</p>	
						</div>	
					</div> 
					
					
				</div>	  <!-- End container -->							
			</footer>	<!-- END FOOTER -->
    </div>
</template>

<style scoped>
</style>
