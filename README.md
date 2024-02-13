## django_snacks Repo

### LAB - Class 26 Project: django_snacks

### Author: DeAndre Ordonez

### Links and Resources - N/A

### Setup - N/A

### PORT - N/A

### DATABASE_URL - N/A

### How to initialize/run your application - 

- `python manage.py runserver`

### How to use your library

`pip install requirements.txt`
`npm install`

### Tests How do you run tests?

`python manage.py test`

### Tested-

```    
    def test_about_page_status_code(self):
        response = self.client.get('/about/')
        self.assertEqual(response.status_code, 200)
        
    def test_home_page_status_code(self):
        url = reverse('home')
        response = self.client.get(url)
        self.assertEqual(response.status_code, 200)

    def test_home_page_templete(self):
        url = reverse('home')
        response = self.client.get(url)
        self.assertTemplateUsed(response, 'home.html')
        self.assertTemplateUsed(response, 'base.html')  
```

### Any tests of note? - N/A

### Describe any tests that you did not complete, skipped, etc - N/A

