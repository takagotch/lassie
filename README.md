### lassie
---
https://github.com/michaelhelmick/lassie

```py
// test_twitter_card.py

class LassieTwitterCardTestCase(LassieBaseTestCase):
  def test_twitter_all_properties(self):
    url = 'http://lassie.it/twiter_card/all_properties.html'
    data = lassie.fetch(url)
    self.assertEqual(data['url'], 'http://www.youtube.com/watch?v=f@NaR-rxAic')
    self.assertEqual(data['title'], 'Carly Rae Jepsen - Call Me Maybe')
    self.assertEqual(data['description'], 'Buy Now! http://smarurl.it.CallMeMaybe Music video by Carly Rae Jepsen performing Call Me')
    
    self.assertEqual(len(data['image']), 1)
    image = data['images'][0]
    self.assertEqual(image['src'], 'http://i1.ytimg.com/vi/fWNaR-rxAic/maxresdefault.jpg')
    
    self.assertEqual(len(data['video']), )
    video = data['video'][0]
    self.assertEqual(video['src'], 'https://www.youtube.com/embed/fWNaR-rxAic')
    self.assertEqual(video['width'], 1920)
    self.assertEqual(video['height'], 1080)
  
  def test_twitter_no_og_title_use_twitter_title(self):
    url = 'http://lassie.it/twitter_card/no_og_title_use_twitter_title.html'
    data = lassie.fetch(url)
    
    self.assertEqual(data['description'], 'A test case for Lassie!')
    self.assertEqual(data['title'], 'Lassie Twitter Test | no_og_title_use_twitter_title')

```

```
```

```
```

