# Template customization


## src
I hope you have seen this template `src` folder on the downloaded package `Prolend - Angular 9 Product Landing Page` from ThemeForest.

In this `src` folder you can see `index.html` file. This file structure is like this-

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <!--meta, title, base, google fonts, all css linking here-->
</head>

<body>

  <app-root></app-root>
 
 <!--all js linking here-->
</body>

</html>
```

All HTML content will be load into this `app-root`:
```html
<app-root></app-root>
```


## entry points

##### app-component.html
Template `app-component.html` structure looks like this-
```html
<router-outlet></router-outlet>

```

##### app-component.ts
Here we have generated all of our components. Template `app-component.ts` structure looks like this-
```js
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'prolend';
}

```

##### app.module.ts
Template `app.module.ts` structure looks like this-
```js
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';

import { AppRoutingModule } from './app-routing.module';
import { AppComponent } from './app.component';
import { WelcomeOneComponent } from './components/welcome/welcome-one/welcome-one.component';
import { WelcomeTwoComponent } from './components/welcome/welcome-two/welcome-two.component';
import { WelcomeThreeComponent } from './components/welcome/welcome-three/welcome-three.component';
import { WelcomeFourComponent } from './components/welcome/welcome-four/welcome-four.component';
import { WelcomeFiveComponent } from './components/welcome/welcome-five/welcome-five.component';
import { WelcomeSixComponent } from './components/welcome/welcome-six/welcome-six.component';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { HeaderOneComponent } from './components/header/header-one/header-one.component';
import { HeaderTwoComponent } from './components/header/header-two/header-two.component';
import { ServiceOneComponent } from './components/service/service-one/service-one.component';
import { ServiceTwoComponent } from './components/service/service-two/service-two.component';
import { ServiceThreeComponent } from './components/service/service-three/service-three.component';
import { ServiceFourComponent } from './components/service/service-four/service-four.component';
import { ServiceFiveComponent } from './components/service/service-five/service-five.component';
import { DiscoverOneComponent } from './components/discover/discover-one/discover-one.component';
import { DiscoverTwoComponent } from './components/discover/discover-two/discover-two.component';
import { DiscoverThreeComponent } from './components/discover/discover-three/discover-three.component';
import { DiscoverFourComponent } from './components/discover/discover-four/discover-four.component';
import { CtaOneComponent } from './components/cta/cta-one/cta-one.component';
import { CtaTwoComponent } from './components/cta/cta-two/cta-two.component';
import { FeaturesOneComponent } from './components/features/features-one/features-one.component';
import { FeaturesTwoComponent } from './components/features/features-two/features-two.component';
import { FeaturesThreeComponent } from './components/features/features-three/features-three.component';
import { ProductsOneComponent } from './components/products/products-one/products-one.component';
import { ProductsTwoComponent } from './components/products/products-two/products-two.component';
import { ComparisonOneComponent } from './components/comparison/comparison-one/comparison-one.component';
import { ComparisonTwoComponent } from './components/comparison/comparison-two/comparison-two.component';
import { DownloadComponent } from './components/download/download.component';
import { ReviewsOneComponent } from './components/reviews/reviews-one/reviews-one.component';
import { ReviewsTwoComponent } from './components/reviews/reviews-two/reviews-two.component';
import { FaqOneComponent } from './components/faq/faq-one/faq-one.component';
import { FaqTwoComponent } from './components/faq/faq-two/faq-two.component';
import { ContactOneComponent } from './components/contact/contact-one/contact-one.component';
import { ContactTwoComponent } from './components/contact/contact-two/contact-two.component';
import { FooterOneComponent } from './components/footer/footer-one/footer-one.component';
import { FooterTwoComponent } from './components/footer/footer-two/footer-two.component';
import { ScrollupComponent } from './components/scrollup/scrollup.component';
import { ThemeTwoComponent } from './themes/theme-two/theme-two.component';
import { ThemeThreeComponent } from './themes/theme-three/theme-three.component';
import { ThemeFourComponent } from './themes/theme-four/theme-four.component';
import { ThemeFiveComponent } from './themes/theme-five/theme-five.component';
import { ThemeSixComponent } from './themes/theme-six/theme-six.component';
import { HeaderThreeComponent } from './components/header/header-three/header-three.component';
import { PromoOneComponent } from './components/promo/promo-one/promo-one.component';
import { PromoTwoComponent } from './components/promo/promo-two/promo-two.component';
import { PromoVideoComponent } from './components/promo-video/promo-video.component';
import { BreadcrumbBlogTwoColumnComponent } from './components/breadcrumb/breadcrumb-blog-two-column/breadcrumb-blog-two-column.component';
import { BreadcrumbBlogThreeColumnComponent } from './components/breadcrumb/breadcrumb-blog-three-column/breadcrumb-blog-three-column.component';
import { BreadcrumbBlogLeftSidebarComponent } from './components/breadcrumb/breadcrumb-blog-left-sidebar/breadcrumb-blog-left-sidebar.component';
import { BreadcrumbBlogRightSidebarComponent } from './components/breadcrumb/breadcrumb-blog-right-sidebar/breadcrumb-blog-right-sidebar.component';
import { BreadcrumbBlogDetailsLeftSidebarComponent } from './components/breadcrumb/breadcrumb-blog-details-left-sidebar/breadcrumb-blog-details-left-sidebar.component';
import { BreadcrumbBlogDetailsRightSidebarComponent } from './components/breadcrumb/breadcrumb-blog-details-right-sidebar/breadcrumb-blog-details-right-sidebar.component';
import { BreadcrumbReviewsComponent } from './components/breadcrumb/breadcrumb-reviews/breadcrumb-reviews.component';
import { BreadcrumbFaqComponent } from './components/breadcrumb/breadcrumb-faq/breadcrumb-faq.component';
import { BreadcrumbContactComponent } from './components/breadcrumb/breadcrumb-contact/breadcrumb-contact.component';
import { BlogTwoColumnComponent } from './components/blogs/blog-two-column/blog-two-column.component';
import { BlogThreeColumnComponent } from './components/blogs/blog-three-column/blog-three-column.component';
import { BlogLeftSidebarComponent } from './components/blogs/blog-left-sidebar/blog-left-sidebar.component';
import { BlogRightSidebarComponent } from './components/blogs/blog-right-sidebar/blog-right-sidebar.component';
import { BlogDetailsLeftSidebarComponent } from './components/blogs/blog-details-left-sidebar/blog-details-left-sidebar.component';
import { BlogDetailsRightSidebarComponent } from './components/blogs/blog-details-right-sidebar/blog-details-right-sidebar.component';
import { ReviewsPageComponent } from './components/inner-pages/reviews-page/reviews-page.component';
import { FaqPageComponent } from './components/inner-pages/faq-page/faq-page.component';
import { ContactPageComponent } from './components/inner-pages/contact-page/contact-page.component';
import { ErrorPageComponent } from './components/inner-pages/error-page/error-page.component';

@NgModule({
  declarations: [
    AppComponent,
    WelcomeOneComponent,
    WelcomeTwoComponent,
    WelcomeThreeComponent,
    WelcomeFourComponent,
    WelcomeFiveComponent,
    WelcomeSixComponent,
    ThemeOneComponent,
    HeaderOneComponent,
    HeaderTwoComponent,
    ServiceOneComponent,
    ServiceTwoComponent,
    ServiceThreeComponent,
    ServiceFourComponent,
    ServiceFiveComponent,
    DiscoverOneComponent,
    DiscoverTwoComponent,
    DiscoverThreeComponent,
    DiscoverFourComponent,
    CtaOneComponent,
    CtaTwoComponent,
    FeaturesOneComponent,
    FeaturesTwoComponent,
    FeaturesThreeComponent,
    ProductsOneComponent,
    ProductsTwoComponent,
    ComparisonOneComponent,
    ComparisonTwoComponent,
    DownloadComponent,
    ReviewsOneComponent,
    ReviewsTwoComponent,
    FaqOneComponent,
    FaqTwoComponent,
    ContactOneComponent,
    ContactTwoComponent,
    FooterOneComponent,
    FooterTwoComponent,
    ScrollupComponent,
    ThemeTwoComponent,
    ThemeThreeComponent,
    ThemeFourComponent,
    ThemeFiveComponent,
    ThemeSixComponent,
    HeaderThreeComponent,
    PromoOneComponent,
    PromoTwoComponent,
    PromoVideoComponent,
    BreadcrumbBlogTwoColumnComponent,
    BreadcrumbBlogThreeColumnComponent,
    BreadcrumbBlogLeftSidebarComponent,
    BreadcrumbBlogRightSidebarComponent,
    BreadcrumbBlogDetailsLeftSidebarComponent,
    BreadcrumbBlogDetailsRightSidebarComponent,
    BreadcrumbReviewsComponent,
    BreadcrumbFaqComponent,
    BreadcrumbContactComponent,
    BlogTwoColumnComponent,
    BlogThreeColumnComponent,
    BlogLeftSidebarComponent,
    BlogRightSidebarComponent,
    BlogDetailsLeftSidebarComponent,
    BlogDetailsRightSidebarComponent,
    ReviewsPageComponent,
    FaqPageComponent,
    ContactPageComponent,
    ErrorPageComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```


## themes

`themes` folder included on `app` folder. You can check our folder structure on `app` folder menu.
This is `themes` folder structure-
```text
|-- themes
    |-- theme-one ( default theme)
    |-- theme-two ( demo theme 2)
    .....
    |-- theme-six ( demo theme 6 )
```

`themes` folder contains all of our 6 demos.


## app-routing
In `app` folder we used `app-routing.module.ts`. Where we linked all the route for our all theme. For routing we used angular-router.

Routes: `src/app/app-routing.module.ts`

```js
import { NgModule } from '@angular/core';
import { Routes, RouterModule } from '@angular/router';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { ThemeTwoComponent } from './themes/theme-two/theme-two.component';
import { ThemeThreeComponent } from './themes/theme-three/theme-three.component';
import { ThemeFourComponent } from './themes/theme-four/theme-four.component';
import { ThemeFiveComponent } from './themes/theme-five/theme-five.component';
import { ThemeSixComponent } from './themes/theme-six/theme-six.component';
import { BlogTwoColumnComponent } from './components/blogs/blog-two-column/blog-two-column.component';
import { BlogThreeColumnComponent } from './components/blogs/blog-three-column/blog-three-column.component';
import { BlogLeftSidebarComponent } from './components/blogs/blog-left-sidebar/blog-left-sidebar.component';
import { BlogRightSidebarComponent } from './components/blogs/blog-right-sidebar/blog-right-sidebar.component';
import { BlogDetailsLeftSidebarComponent } from './components/blogs/blog-details-left-sidebar/blog-details-left-sidebar.component';
import { BlogDetailsRightSidebarComponent } from './components/blogs/blog-details-right-sidebar/blog-details-right-sidebar.component';
import { ReviewsPageComponent } from './components/inner-pages/reviews-page/reviews-page.component';
import { FaqPageComponent } from './components/inner-pages/faq-page/faq-page.component';
import { ContactPageComponent } from './components/inner-pages/contact-page/contact-page.component';
import { ErrorPageComponent } from './components/inner-pages/error-page/error-page.component';



const routes: Routes = [
  {path: '', component: ThemeOneComponent},
  {path: 'theme-two', component: ThemeTwoComponent},
  {path: 'theme-three', component: ThemeThreeComponent},
  {path: 'theme-four', component: ThemeFourComponent},
  {path: 'theme-five', component: ThemeFiveComponent},
  {path: 'theme-six', component: ThemeSixComponent},
  {path: 'blog-two-column', component: BlogTwoColumnComponent},
  {path: 'blog-three-column', component: BlogThreeColumnComponent},
  {path: 'blog-left-sidebar', component: BlogLeftSidebarComponent},
  {path: 'blog-right-sidebar', component: BlogRightSidebarComponent},
  {path: 'blog-details-left-sidebar', component: BlogDetailsLeftSidebarComponent},
  {path: 'blog-details-right-sidebar', component: BlogDetailsRightSidebarComponent},
  {path: 'reviews-page', component: ReviewsPageComponent},
  {path: 'faq-page', component: FaqPageComponent},
  {path: 'contact-page', component: ContactPageComponent},
  {path: 'error-page', component: ErrorPageComponent}
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }

```


## components
Under `components` folder we generated all of our components individually. 
We have generated these components to make the developer’s life easy. 
By using these basic components, For example in our components directory there is `header`, `welcome` , `footer` folder where we wrote our different styled component. For example `welcome` component-

### Component folder structure
```text
|-- components
    ....
    ..
    |-- welcome ( welcome component folder )
        - welcome-one ( main demo welcome section )
        - welcome-two ( demo two welcome section )
        ...... ( and other )
    ...    
```
### Welcome One Page component
`components/welcome/welcome-one/welcome-one.component.html`

```html
<section id="home" class="section welcome-area bg-inherit h-100vh overflow-hidden">
    <div class="shapes-container">
        <div class="bg-shape"></div>
    </div>
    <div class="container h-100">
        <div class="row align-items-center h-100">
            <!-- Welcome Intro Start -->
            <div class="col-12 col-md-7">
                <div class="welcome-intro">
                    <span class="d-inline-block text-capitalize font-italic fw-3 mb-2">The next generation landing page</span>
                    <h1 class="text-capitalize">Get <span class="fw-3">Prolend</span> Product landing page</h1>
                    <p class="my-4">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p>
                    <!-- Store Buttons -->
                    <div class="button-group store-buttons d-flex">
                        <a class="btn prolend-primary" href="#">Get the App</a>
                        <a class="btn prolend-primary style-two" href="#">Learn More</a>
                    </div>
                </div>
            </div>
            <div class="col-12 col-md-5">
                <!-- Welcome Thumb -->
                <div class="welcome-thumb thumb-animated">
                    <img src="assets/img/welcome_mockup.png" alt="">
                </div>
            </div>
        </div>
    </div>
</section>
```

### Blog Page component
`components/blogs/blog-two-column/blog-two-column.component.html`

```html
<div class="blog">
    <app-scrollup></app-scrollup>
    <div class="main">
        <app-header-two></app-header-two>
        <app-breadcrumb-blog-two-column></app-breadcrumb-blog-two-column>
        <section id="blog" class="section blog-area ptb_100">
            <div class="container">
                <div class="row">
                    <div class="col-12 col-md-6">
                        <!-- Single Blog -->
                        <div class="single-blog res-margin">
                            <!-- Blog Thumb -->
                            <div class="blog-thumb">
                                <a href="#"><img src="assets/img/blog_1.jpg" alt=""></a>
                            </div>
                            <!-- Blog Content -->
                            <div class="blog-content p-4">
                                <!-- Meta Info -->
                                <ul class="meta-info d-flex justify-content-between">
                                    <li>By <a href="#">Anna Sword</a></li>
                                    <li><a href="#">Feb 05, 2019</a></li>
                                </ul>
                                <!-- Blog Title -->
                                <h3 class="blog-title my-3"><a href="#">How to grow up your business</a></h3>
                                <p>It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution.</p>
                                <a href="#" class="blog-btn mt-3">Read More</a>
                            </div>
                        </div>
                    </div>
                    <div class="col-12 col-md-6">
                        <!-- Single Blog -->
                        <div class="single-blog res-margin">
                            <!-- Blog Thumb -->
                            <div class="blog-thumb">
                                <a href="#"><img src="assets/img/blog_2.jpg" alt=""></a>
                            </div>
                            <!-- Blog Content -->
                            <div class="blog-content p-4">
                                <!-- Meta Info -->
                                <ul class="meta-info d-flex justify-content-between">
                                    <li>By <a href="#">Jassica William</a></li>
                                    <li><a href="#">Feb 05, 2019</a></li>
                                </ul>
                                <!-- Blog Title -->
                                <h3 class="blog-title my-3"><a href="#">Planing to manage your clients?</a></h3>
                                <p>Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. Richard McClintock, a Latin professor.</p>
                                <a href="#" class="blog-btn mt-3">Read More</a>
                            </div>
                        </div>
                    </div>
                    <div class="col-12 col-md-6">
                        <!-- Single Blog -->
                        <div class="single-blog">
                            <!-- Blog Thumb -->
                            <div class="blog-thumb">
                                <a href="#"><img src="assets/img/blog_3.jpg" alt=""></a>
                            </div>
                            <!-- Blog Content -->
                            <div class="blog-content p-4">
                                <!-- Meta Info -->
                                <ul class="meta-info d-flex justify-content-between">
                                    <li>By <a href="#">John Doe</a></li>
                                    <li><a href="#">Mar 05, 2019</a></li>
                                </ul>
                                <!-- Blog Title -->
                                <h3 class="blog-title my-3"><a href="#">Make your successful business with Prolend</a></h3>
                                <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable. If you are going to use a passage.</p>
                                <a href="#" class="blog-btn mt-3">Read More</a>
                            </div>
                        </div>
                    </div>
                    <div class="col-12 col-md-6">
                        <!-- Single Blog -->
                        <div class="single-blog res-margin">
                            <!-- Blog Thumb -->
                            <div class="blog-thumb">
                                <a href="#"><img src="assets/img/blog_4.jpg" alt=""></a>
                            </div>
                            <!-- Blog Content -->
                            <div class="blog-content p-4">
                                <!-- Meta Info -->
                                <ul class="meta-info d-flex justify-content-between">
                                    <li>By <a href="#">Anna Sword</a></li>
                                    <li><a href="#">Feb 05, 2019</a></li>
                                </ul>
                                <!-- Blog Title -->
                                <h3 class="blog-title my-3"><a href="#">How to get more clients?</a></h3>
                                <p>Need to be sure there isn't anything embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary, making this the first true generator on the Internet.</p>
                                <a href="#" class="blog-btn mt-3">Read More</a>
                            </div>
                        </div>
                    </div>
                    <div class="col-12 col-md-6">
                        <!-- Single Blog -->
                        <div class="single-blog res-margin">
                            <!-- Blog Thumb -->
                            <div class="blog-thumb">
                                <a href="#"><img src="assets/img/blog_5.jpg" alt=""></a>
                            </div>
                            <!-- Blog Content -->
                            <div class="blog-content p-4">
                                <!-- Meta Info -->
                                <ul class="meta-info d-flex justify-content-between">
                                    <li>By <a href="#">Jassica William</a></li>
                                    <li><a href="#">Feb 05, 2019</a></li>
                                </ul>
                                <!-- Blog Title -->
                                <h3 class="blog-title my-3"><a href="#">Grow up your business successfully</a></h3>
                                <p>Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. Richard McClintock, a Latin professor.</p>
                                <a href="#" class="blog-btn mt-3">Read More</a>
                            </div>
                        </div>
                    </div>
                    <div class="col-12 col-md-6">
                        <!-- Single Blog -->
                        <div class="single-blog">
                            <!-- Blog Thumb -->
                            <div class="blog-thumb">
                                <a href="#"><img src="assets/img/blog_6.jpg" alt=""></a>
                            </div>
                            <!-- Blog Content -->
                            <div class="blog-content p-4">
                                <!-- Meta Info -->
                                <ul class="meta-info d-flex justify-content-between">
                                    <li>By <a href="#">John Doe</a></li>
                                    <li><a href="#">Mar 05, 2019</a></li>
                                </ul>
                                <!-- Blog Title -->
                                <h3 class="blog-title my-3"><a href="#">Meet the business magnet of the year</a></h3>
                                <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly</p>
                                <a href="#" class="blog-btn mt-3">Read More</a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="row">
                    <div class="col-12">
                        <!-- Pagination -->
                        <ul class="pagination justify-content-center">
                            <li class="disabled px-1">
                                <a href="#" aria-label="Previous">
                                    <i class="fas fa-arrow-left"></i>
                                </a>
                            </li>
                            <li class="px-1"><a href="#">1</a></li>
                            <li class="active px-1"><a href="#">2</a></li>
                            <li class="px-1"><a href="#">3</a></li>
                            <li>
                                <a href="#" aria-label="Next">
                                    <i class="fas fa-arrow-right"></i>
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>
        <app-footer-two></app-footer-two>
    </div>
</div>
```

### Contact Page component
`inner-pages/contact-page/contact-page.component.html`

```text
|-- components
    ....
    ..
    |-- inner-pages ( all inner-pages folder )
        ......
        - contact-page ( contact-page component )
        ...... ( and other )
    ...    
```

```html
<div class="contact-page">
    <app-scrollup></app-scrollup>
    <div class="main">
        <app-header-two></app-header-two>
        <app-breadcrumb-contact></app-breadcrumb-contact>
        <app-contact-two></app-contact-two>
        <section class="section map-area">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2485.596666220624!2d-0.16124461362595294!3d51.46556134684942!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x487605a25375dfb7%3A0xe0d9fa09dcf932a8!2s15%20Theatre%20St%2C%20Battersea%2C%20London%20SW11%205ND%2C%20UK!5e0!3m2!1sen!2sbd!4v1567427969685!5m2!1sen!2sbd" width="100" height="100" style="border:0;" allowfullscreen=""></iframe>
        </section>
        <app-footer-one></app-footer-one>
    </div>
</div>
```

### Editing the style CSS
`src/assets/css/style.css`

```css
/* ************************************************************
:: Template Name: Prolend - Product Landing Page Template
:: Template URI: https://theme-land.com/prolend
:: Template Author Name: theme_land
:: Template Author URI: hridoy1272@gmail.com
:: Version: 1.0.0
:: Created: 14 Jun 2020
************************************************************ 
*
*
******* :: INDEX OF CSS :: *******
:: 1.0 WEB FONTS
:: 2.0 IMPORT ALL CSS
:: 3.0 GLOBAL CSS
:: 4.0 COMMON CSS
:: 5.0 PRELOADER CSS
:: 6.0 SCROLL TO TOP AREA CSS
:: 7.0 HEADER AREA CSS
:: 8.0 WELCOME AREA CSS
    :: 8.1 WELCOME AREA HOMEPAGE-2 CSS
    :: 8.2 WELCOME AREA HOMEPAGE-3 CSS
    :: 8.3 WELCOME AREA HOMEPAGE-4 CSS
    :: 8.4 WELCOME AREA HOMEPAGE-6 CSS
:: 9.0 PROMO VIDEO AREA CSS
:: 10.0 FEATURES AREA CSS
:: 11.0 SERVICE AREA CSS
:: 12.0 DISCOVER AREA CSS
:: 13.0 PRODUCTS AREA CSS
:: 14.0 COMPARISON AREA CSS
:: 15.0 REVIEWS AREA CSS
:: 16.0 FAQ AREA CSS
:: 17.0 SUBSCRIBE AREA CSS
:: 18.0 BLOG AREA CSS
:: 19.0 BREADCRUMB AREA CSS
:: 20.0 BLOG PAGE AREA CSS
:: 21.0 BLOG PAGE DETAILS AREA CSS
:: 22.0 CONTACT AREA CSS
:: 23.0 FOOTER AREA CSS
:: 24.0 ERROR AREA CSS
:: 25.0 COMING SOON AREA CSS
:: 26.0 PREVIEW AREA CSS
****************************** */

/* ******************************
:: 1.0 WEB FONTS
****************************** */
@import url('https://fonts.googleapis.com/css?family=Poppins:300,400,500,600,700&display=swap');

/* ******************************
:: 2.0 IMPORT ALL CSS
****************************** */
@import url(bootstrap.min.css);
@import url(all.min.css);
@import url(../font/flaticon.css);
@import url(animate.min.css);
@import url(aos.css);
@import url(owl.carousel.min.css);
@import url(slick.css);
@import url(jquery.fancybox.min.css);

/* ******************************
:: 3.0 GLOBAL CSS
****************************** */
* {
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Poppins', sans-serif;
    font-size: 14px;
    line-height: 24px;
    font-weight: 400;
    color: #565656;
}

.main {
    background: #fff;
}

section,
.section {
    position: relative;
}

.container {
    width: 100%;
    margin: 0 auto;
}

h1,
h2,
h3,
.h3,
h4,
h5,
h6 {
    font-weight: 600;
    color: #222;
    margin-bottom: 0;
}

h1 {
    font-size: 4em;
    font-weight: 600;
    line-height: 1.2;
}

h2 {
    font-size: 40px;
    line-height: 1.3;
}

@media (min-width: 992px) {
    .promo-text {
        font-size: 50px;
    }
}

h3, .h3 {
    font-size: 20px;
    line-height: 1.2;
}

h4 {
    font-size: 20px;
}

h5 {
    font-size: 16px;
}

h6 {
    font-size: 14px;
    font-weight: 400;
}

p {
    font-size: 14px;
    font-weight: 400;
    line-height: 24px;
    color: #565656;
    margin-bottom: 0;
}

a {
    color: #444;
    -webkit-transition: all 0.3s ease 0s;
    transition: all 0.3s ease 0s;
}

a:hover,
a:focus {
    color: #F74B54;
}

a,
a:hover,
a:focus,
.btn:focus {
    text-decoration: none;
    outline: none;
    -webkit-box-shadow: none;
    box-shadow: none;
}
```


## theme installtion
To install the theme you have to install [angular](https://cli.angular.io/) than go to the theme root dir where `package.json` located and use
```bash
npm install -g @angular/cli
```
it will install the packages.

After install process now you can run local server- local server port is 'http://localhost:4200' For developement start use
```bash
ng serve -o
```
## Build your theme
```bash
ng build --prod
```

## For deployment -- static server
First install
```bash
ng build --watch
ng build --aot
```
If you want to know more about static deployment please visit [Angular app deployment](https://angular.io/guide/deployment)

Enjoy your theme :)
