Check box buttons --> https://bootsnipp.com/snippets/featured/jquery-checkbox-buttons

  HTML in app/views/calendar.html.erb
  JS in app/assets/javascripts/application.js

Used Le Wagon minimal template --> https://github.com/lewagon/rails-templates

------------------------------------------------------------------------------------------------------------


<% array = date_range.each_slice(14).to_a %>
        <% weekarray = array[0] %>
        <p>date range</p> <%= date_range %>
        <p>week</p> <%= week %> <br>
        <p>weekarray</p> <%= weekarray %> <br>


>> week
=> [Mon, 15 May 2017, Tue, 16 May 2017, Wed, 17 May 2017, Thu, 18 May 2017, Fri, 19 May 2017, Sat, 20 May 2017, Sun, 21 May 2017]

>> date_range.each_slice(14)
=> #<Enumerator: [Mon, 15 May 2017, Tue, 16 May 2017, Wed, 17 May 2017, Thu, 18 May 2017, Fri, 19 May 2017, Sat, 20 May 2017, Sun, 21 May 2017, Mon, 22 May 2017, Tue, 23 May 2017, Wed, 24 May 2017, Thu, 25 May 2017, Fri, 26 May 2017, Sat, 27 May 2017, Sun, 28 May 2017]:each_slice(14)>


>> array = date_range.each_slice(14).to_a
=> [[Mon, 15 May 2017, Tue, 16 May 2017, Wed, 17 May 2017, Thu, 18 May 2017, Fri, 19 May 2017, Sat, 20 May 2017, Sun, 21 May 2017, Mon, 22 May 2017, Tue, 23 May 2017, Wed, 24 May 2017, Thu, 25 May 2017, Fri, 26 May 2017, Sat, 27 May 2017, Sun, 28 May 2017]]


>> array
=> [[Mon, 15 May 2017, Tue, 16 May 2017, Wed, 17 May 2017, Thu, 18 May 2017, Fri, 19 May 2017, Sat, 20 May 2017, Sun, 21 May 2017, Mon, 22 May 2017, Tue, 23 May 2017, Wed, 24 May 2017, Thu, 25 May 2017, Fri, 26 May 2017, Sat, 27 May 2017, Sun, 28 May 2017]]

>> array = array[0]
=> [Mon, 15 May 2017, Tue, 16 May 2017, Wed, 17 May 2017, Thu, 18 May 2017, Fri, 19 May 2017, Sat, 20 May 2017, Sun, 21 May 2017, Mon, 22 May 2017, Tue, 23 May 2017, Wed, 24 May 2017, Thu, 25 May 2017, Fri, 26 May 2017, Sat, 27 May 2017, Sun, 28 May 2017]

>> array
=> [Mon, 15 May 2017, Tue, 16 May 2017, Wed, 17 May 2017, Thu, 18 May 2017, Fri, 19 May 2017, Sat, 20 May 2017, Sun, 21 May 2017, Mon, 22 May 2017, Tue, 23 May 2017, Wed, 24 May 2017, Thu, 25 May 2017, Fri, 26 May 2017, Sat, 27 May 2017, Sun, 28 May 2017]

>> week
=> [Mon, 15 May 2017, Tue, 16 May 2017, Wed, 17 May 2017, Thu, 18 May 2017, Fri, 19 May 2017, Sat, 20 May 2017, Sun, 21 May 2017]

------------------------------------------------------------------------------------------------------------------
