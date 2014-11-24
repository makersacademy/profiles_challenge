Profile Challenge
==================

Here's an analysis of the Github accounts of the August cohort:

http://blog.makersacademy.com/what-our-makers-make/

Your challenge is to do a similar analysis on your own Github. What's the breakdown of languages you use? How many commits have you logged during your time at Makers? What words appear most in your commit messages? Etc.

To accomplish this you'll need to leverage Github's API. The docs are great. Here are some features that might be helpful:

* http://developer.github.com/v3/repos/statistics/
* http://developer.github.com/v3/repos/commits/
* http://developer.github.com/v3/repos/#list-languages

To fetch data from the API you have a couple of options. Using a HTTP library like Net::HTTP (comes with Ruby) or HTTParty (https://github.com/jnunemaker/httparty). Octokit.rb is a gem specifically designed around interacting with the Github API (https://github.com/octokit/octokit.rb).

Once you've done your own Github, write a simple program to which you can provide an arbitrary Github username and get the statistics for that user.

Write tests for your application. Start off by actually fetching the data from the Github API in your tests (which will be slow!), then have a look at something like Webmock (https://github.com/bblimke/webmock) to avoid making real HTTP requests.

Good luck :)
