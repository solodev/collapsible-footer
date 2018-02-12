# collapsible-footer
There’s a ton of information floating around about the ‘perfect landing page,’ but don’t forget about your website’s most important page -- the pricing page! Design can boost your pricing strategy by a few visual tricks and simple SCSS. And while this tutorial isn’t a one-size-fits-all solution, it can definitely help boost your click through rate and (hopefully) your bottom line!
  		  
## Tutorial		  
For detailed instruction's, view Solodev's [How to Design Pricing Boxes that Get People to Click](https://www.solodev.com/blog/how-to-design-pricing-boxes-that-get-people-to-click-.stml) article.
 
## Demo
  		  
Try out a working example on [JSFiddle](https://jsfiddle.net/solodev/zne97LcL/).

## HTML

The tutorial contains the following basic HTML markup.

```

<footer class="footer-collapse px-1 py-3">
    <div class="col-lg-9 mx-auto">
            <h2 class="sr-only">Solodev Content Management System</h2>
            <div class="row">
                <div class="col-sm-6 col-md-3">
                    <div class="widget hidden-xs-down">
                    <h4 class="text-uppercase text-bold">Product</h4>
                    <ul class="widget-list list-unstyled p-0">
                        <li><a href="https://www.solodev.com/product/create.stml">Create Websites</a></li>
                        <li><a href="https://www.solodev.com/product/host.stml">Secure Cloud Hosting</a></li>
                        <li><a href="https://www.solodev.com/product/engage.stml">Engage Your Audience</a></li>
                        <li><a href="https://www.solodev.com/product/support.stml">Website Support</a></li>
                    </ul>
                    </div>
                    <div id="accordion" role="tablist" aria-multiselectable="true" class="widget hidden-sm-up">
                    <div role="tab" id="headingOne">
                        <h4 class="card-header py-3 border-0 text-uppercase text-bold">
                        <a data-toggle="collapse" data-parent="#accordion" href="#collapseOne" aria-expanded="false" aria-controls="collapseOne">
                            Product
                        </a>
                        </h4>
                    </div>
                    <div id="collapseOne" class="collapse" role="tabpanel" aria-labelledby="headingOne">
                        <div class="card-block">
                        <ul class="widget-list list-unstyled p-0">
                            <li><a href="https://www.solodev.com/product/create.stml">Create Websites</a></li>
                            <li><a href="https://www.solodev.com/product/host.stml">Secure Cloud Hosting</a></li>
                            <li><a href="https://www.solodev.com/product/engage.stml">Engage Your Audience</a></li>
                            <li><a href="https://www.solodev.com/product/support.stml">Website Support</a></li>
                        </ul>
                        </div>
                    </div>
                    </div>
                </div>
                <div class="col-sm-6 col-md-3">
                    <div class="widget hidden-xs-down">
                        <h4 class="text-uppercase text-bold">Company</h4>
                        <ul class="widget-list list-unstyled p-0">
                            <li><a href="https://www.solodev.com/company/">About</a></li>
                            <li><a href="https://www.solodev.com/careers/">Careers</a></li>
                            <li><a href="http://solodev.zendesk.com" target="_blank">Support</a></li>
                            <li><a href="https://www.solodev.com/pricing/">Pricing</a></li>
                            <li><a href="https://www.solodev.com/pricing#faq">FAQ</a></li>
                        </ul>
                        </div>
                        <div id="accordion" role="tablist" aria-multiselectable="true" class="widget hidden-sm-up">
                        <div role="tab" id="headingTwo">
                            <h4 class="card-header py-3 border-0 text-uppercase text-bold">
                            <a data-toggle="collapse" data-parent="#accordion" href="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                                Company
                            </a>
                            </h4>
                        </div>
                        <div id="collapseTwo" class="collapse" role="tabpanel" aria-labelledby="headingTwo">
                            <div class="card-block">
                                <ul class="widget-list list-unstyled">
                                    <li><a href="https://www.solodev.com/company/">About</a></li>
                                    <li><a href="https://www.solodev.com/careers/">Careers</a></li>
                                    <li><a href="http://solodev.zendesk.com" target="_blank">Support</a></li>
                                    <li><a href="https://www.solodev.com/pricing/">Pricing</a></li>
                                    <li><a href="https://www.solodev.com/pricing#faq">FAQ</a></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-sm-6 col-md-3">
                    <div class="widget hidden-xs-down">
                        <h4 class="text-uppercase text-bold">Resources</h4>
                        <ul class="widget-list list-unstyled p-0">
                            <li><a href="https://www.solodev.com/blog/">Blog</a></li>
                            <li><a href="https://www.solodev.com/resources/ebooks/">eBooks</a></li>
                            <li><a href="https://www.solodev.com/resources/whitepapers/">Whitepapers</a></li>
                            <li><a href="https://www.solodev.com/comparison-guide/index.stml">Comparison Guide</a></li>
                            <li><a href="https://www.solodev.com/grader/">Website Grader</a></li>
                        </ul>
                        </div>
                        <div id="accordion" role="tablist" aria-multiselectable="true" class="widget hidden-sm-up">
                            <div role="tab" id="headingThree">
                                <h4 class="card-header py-3 border-0 text-uppercase text-bold">
                                <a data-toggle="collapse" data-parent="#accordion" href="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                                    Resources
                                </a>
                                </h4>
                            </div>
                        <div id="collapseThree" class="collapse" role="tabpanel" aria-labelledby="headingThree">
                            <div class="card-block">
                                <ul class="widget-list list-unstyled p-0">
                                    <li><a href="https://www.solodev.com/blog/">Blog</a></li>
                                    <li><a href="https://www.solodev.com/resources/ebooks/">eBooks</a></li>
                                    <li><a href="https://www.solodev.com/resources/whitepapers/">Whitepapers</a></li>
                                    <li><a href="https://www.solodev.com/comparison-guide/index.stml">Comparison Guide</a></li>
                                    <li><a href="https://www.solodev.com/grader/">Website Grader</a></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-sm-6 col-md-3">
                    <div class="widget hidden-xs-down">
                        <h4 class="text-uppercase text-bold">Get Help</h4>
                        <ul class="widget-list list-unstyled list-unstyle p-0">
                            <li><a href="https://solodev.zendesk.com/hc/en-us" target="_blank">Help Center</a></li>
                            <li><a href="https://www.solodev.com/contact/">Contact Us</a></li>
                            <li><a href="https://www.solodev.com/terms/privacy-policy.stml">Privacy Policy</a></li>
                            <li><a href="https://www.solodev.com/terms/">Terms</a></li>
                            <!--<li><a href="/login.stml">Login</a></li>-->
                        </ul>
                    </div>
                    <div id="accordion" role="tablist" aria-multiselectable="true" class="widget hidden-sm-up">
                        <div role="tab" id="headingFour">
                            <h4 class="card-header py-3 border-0 text-uppercase text-bold">
                            <a data-toggle="collapse" data-parent="#accordion" href="#collapseFour" aria-expanded="false" aria-controls="collapseFour">
                                Get Help
                            </a>
                            </h4>
                        </div>
                        <div id="collapseFour" class="collapse" role="tabpanel" aria-labelledby="headingFour">
                            <div class="card-block">
                                <ul class="widget-list list-unstyled p-0">
                                    <li><a href="https://solodev.zendesk.com/hc/en-us" target="_blank">Help Center</a></li>
                                    <li><a href="https://www.solodev.com/contact/">Contact Us</a></li>
                                    <li><a href="https://www.solodev.com/terms/privacy-policy.stml">Privacy Policy</a></li>
                                    <li><a href="https://www.solodev.com/terms/">Terms</a></li>
                                    <!--<li><a href="/login.stml">Login</a></li>-->
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
</footer>
```

## CSS

All required SCSS is contained with collapsible-footer.scss


## External Resources

This tutorial includes the following third party resources.

```
<link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/css/bootstrap.min.css" rel="stylesheet">
<script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/js/bootstrap.min.js"></script>


```

