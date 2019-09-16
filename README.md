### lassie
---
https://github.com/michaelhelmick/lassie

```py
// test_twitter_card.py

class LassieTwitterCardTestCase(LassieBaseTestCase):
  def test_twitter_all_properties(self):
    url = ''
    data = lassie.fetch()
    self.assertEqual()
    self.assertEqual()
    self.assertEqual()
    
    self.assertEqual()
    image = data[][]
    self.assertEqual()
    
    self.assertEqual(len(data['video']), )
    video = data['video'][0]
    self.assertEqual(video[], 'https://www.youtube.com/embed/fWNaR-rxAic')
    self.assertEqual(video[], 1920)
    self.assertEqual(video[], 1080)
  
  def test_twitter_no_og_title_use_twitter_title(self):
    url = ''
    data = lassie.fetch(url)
    
    self.assertEqual(data['description'], 'A test case for Lassie!')
    self.assertEqual(data['title'], 'Lassie Twitter Test | no_og_title_use_twitter_title')

```

```
```

```
```

