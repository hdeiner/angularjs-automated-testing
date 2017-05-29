# Automated AngularJS Testing With Protractor and Karma

I will start with a project written up on a blog at http://mherman.org/blog/2015/04/09/testing-angularjs-with-protractor-and-karma-part-1/ .  The author is demonstrating how AngularJS applications can be unit and end-to-end tested with a variety of tools, including Karma (a test runner), Chai (an assertation framework), Mocha (a unit test tool), and Protractor (for end-to-end browser testing using Selenium).

He shows how we do this testing by hand by doing the following:
1. Install dependencies - 'npm install', followed by 'bower install'
1. Run the development server - `gulp`  You should now be able to run the application in your browser at http://localhost:8888
1. Run unit tests - 'gulp unit`
1. Run e2e tests - in one window, start selenium with 'webdriver-manager start', in another start the application with 'gulp', and in a third window, run the e2e tests with 'gulp e2e`

While this testing is necessary, how about automating the testing and making it possible to run this on a CI server, just like the first class citizens of the Java world?  In other words, manual testing may be necessary, but it is not sufficient for software craftsmanship and quality.

