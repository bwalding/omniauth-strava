omniauth-strava
===============

omniauth strategy for strava 


Configuration
=============

Add the following to your config/initializers/omniauth.rb configuration file:

    Rails.application.config.middleware.use OmniAuth::Builder do

      ...
      
      provider :strava, 'client-id',       'client-secret', {
        scope: 'public' #http://strava.github.io/api/v3/oauth/#get-authorize
      }

    end
