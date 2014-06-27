# jQuery

## jQuery DOM

```
$('#bewareButton').click (event) ->
  $('h1').html('BOOM!!')

$('h1').append("BOOM!!!")
```

```
<div class="germany">
  <h1>Champion</h1>
  <p>2014</p>
  <div class="match">
    <p class="result">Germany wins</p>
    <p>Germany played a good game, Muller got 3 goals so far!</p>
  </div>
</div>

$('.germany h1').html()
$('div.germany h1').html()
$('.germany h2').html()
$('.germany p').html()
$('.germany .match p.result').html()
```

## jQuery AJAX

- Asynchronous
- HTTP methods (GET / POST / PUT / DELETE)

```
response = $.ajax(
  "http://www.omdbapi.com/?s=Matrix"
  dataType: "json"
)

response.done (data) ->
  movies = data.Search
  for movie in movies
    li = "<li><a href='#' data-imdbid='#{movie.imdbID}'>#{movie.Title}</a></li>"
    $('.movies').append(li)
  $('a').click (e) ->
    imdbID = $(@).data('imdbid')

    $.ajax(
      "http://www.omdbapi.com/?i=#{imdbID}&plot=full"
      dataType: "json"
    ).done (data) ->
```

## JSON

- JavaScript Object Notation

```
{
    staff: {
        id: 1,
        name: 'Harry',
        salary_rate: 'poor'
    }
}
```

# Code Challenge

Build a API for Open Movie Database (OMDB)

```
<script type="text/javascript">

// IMDb ID to Search
var imdbId = "tt1285016";

// Send Request
var http = new ActiveXObject("Microsoft.XMLHTTP");
http.open("GET", "http://www.omdbapi.com/?i=" + imdbId, false);
http.send(null);

// Response to JSON
var omdbData = http.responseText;
var omdbJSON = eval("(" + omdbData + ")");

// Returns Movie Title
alert(omdbJSON.Title);

</script>
```

## Resources

- http://www.omdbapi.com/

## Very Old Website
