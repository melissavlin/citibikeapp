citibikeapp
===========

A Citibike helper that provides a list of close-by stations with bike/dock availability overview. Currently the rush hour warning system is being implemented. In the near future I will add "saved locations" functionality so users can convieniently pull up their saved lists such as "Home stations" & "Work stations."

Comments are welcomed. Please pardon the extremely messy and unreadable codes before release. A major code clean-house will be performed once it's ready for the real world.  

To Fork/Clone

First, turn on Postgresql

bundle install
rake db:create
rake db:migrate
rails c
require './dbcitibike.rb'

Also, in Station_controller line 19~22. Make sure line 22 is commented, and line 19 is un-commented. This is due to my own database discrepancies with production db. 
