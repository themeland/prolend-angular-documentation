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
