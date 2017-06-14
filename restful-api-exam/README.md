# RESTful API exam

You should create:
- a MVC architecture
- a database with models 
- controllers
- GET requests
- when you do a GET request, you should return JSON responses 
- tests for your controllers and models - TDD x BDD

The following routes should return JSON response:

- /campaigns
- /ad_groups
- /expanded_text_ad

Please host your demo on Heroku and send Vitor your project on Skype/email.

``` ruby
# Create a restful API based on this JSON response

campaigns = [
  {
    :id => '1',
    :name => 'Interplanetary Cruise',
    :status => 'PAUSED',
    :budget => '3000',
    :advertising_channel_type => 'SEARCH'
  },
  {
    :id => '2',
    :name => 'Police Station',
    :status => 'ON',
    :budget => '2000',
    :advertising_channel_type => 'DISPLAY'
  }
]

ad_groups = [
  {
    :id  => '1', 
    :name => 'Facebook Ads - Napice',
    :status => 'ENABLED',
    :campaign_id => '1'
  },
  {
    :id  => '2', 
    :name => 'Google Ads - Napice',
    :status => 'ENABLED',
    :campaign_id => '1'
  },
  {
    :id  => '3', 
    :name => 'Yahoo Ads - Spotify',
    :status => 'OFFLINE',
    :campaign_id => '2'
  }
]

expanded_text_ad = [
  {
    :xsi_type => 'ExpandedTextAd',
    :ad_group_id => '1',
    :headline_part1 => 'Developers from Mars',
    :headline_part2 => '',
    :description => 'Buy your tickets now!',
    :path1 => 'all-inclusive',
    :path2 => 'deals'
  },
  {
    :xsi_type => 'ExpandedTextAd',
    :ad_group_id => '3',
    :headline_part1 => 'We are looking for the best designers',
    :headline_part2 => 'Best in the galaxy',
    :description => 'We are a team of product builders and are looking for designers',
    :path1 => 'all-inclusive',
    :path2 => 'deals'
  }
]
```
