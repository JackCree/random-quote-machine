# random-quote-machine

## Exercice with [FreeCodeCamp Mooc](https://www.freecodecamp.org/learn/front-end-libraries/front-end-libraries-projects/build-a-random-quote-machine)
Following the exercices of thre Front End librairies certification on FreeCodeCamp, Here is the first exercice done with SASS

##Challenge to make : 
Create a random quote machine with a Json file...
```javascript
function getQuotes() {
  return $.ajax({
    headers: {
      Accept: 'application/json'
    },
    url:
      'https://raw.githubusercontent.com/JackCree/random-quote-machine/main/quotes.json',
    success: function (jsonQuotes) {
      if (typeof jsonQuotes === 'string') {
        quotesData = JSON.parse(jsonQuotes);
        console.log('quotesData');
        console.log(quotesData);
      }
    }
  });
}
```
and HTML incrementation with Javascript
```javascript
$('.quote-text').animate({ opacity: 0 }, 500, function () {
    $(this).animate({ opacity: 1 }, 500);
    $('#text').text(randomQuote.quote);
  });

  $('.quote-author').animate({ opacity: 0 }, 500, function () {
    $(this).animate({ opacity: 1 }, 500);
    $('#author').html(randomQuote.author);
  });
```
