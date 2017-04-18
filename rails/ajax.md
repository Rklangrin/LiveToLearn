# Making Ajax requests with Rails
## What is happening?

**OVERVIEW**

In rails, the Ajax request starts from the HTML that is initially loaded to the page. You can add an option, `remote: true` to the `form_for`/`button_to`/`link_to` view helpers. This will alter the type of request that is made to the server. You can see the difference in the dev tools if you look at the request-accept header (under the network tab), which tells the server what type of information it wants in return. `Remote: true` changes the accept header from requesting HTML to JS. 

So now the server knows the client(the chrome browser) wants information back in the form of javascript. On the controller, you can add different options for how the server responds to different requests using the `respond_to` method. 

```ruby
class AttendanceController < ApplicationController
  
  def create
    @attendance = Attendance.new(attendance_params)
  
    respond_to do |format|
      if @attendance.save
        format.html { redirect_to :back }
        format.js { }
      else ...
```

The `respond_to` method takes a block as seen above. If the requested format is html then the `{ redirect_to :back }` block will run. If the requested format is javascript, then you probably are noticing that the block is empty. Rails will know to look for a file in the views/attendances folder (since you are in the AttendanceController) for a file called create.js.erb (since you are in the create method within the Attendance Controller). The server will send back to the client whatever Javascript is in the create.js.erb file.
