Hi there, I am trying a simple app using erb and sinatra, but I am keep on getting this error messege :
"wrong number of arguments (1 for 0) 
here is index.erb code

```
<form action="/search" method="POST">
   <select name="search_by">
       <option value="id">Id</option>
       <option value="name">Name</option>
       <option value="evilness">evilness</option>
   </select>
   <input type="text" name="searchterm">
   <button type="submit">Search</button>
 </form>
 
 and here is app.rb code
 ```
 post '/search' do
  varx = params [:search_by]
  vary = params [:searchterm]
  cat = Cat.new
  cag.find(vary)
  erb :cat
end
