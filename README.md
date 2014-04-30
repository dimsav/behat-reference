Behat Reference
===============


## Mink

### Radio button

Select a radio button

```php
$this->selectOption('my_name', 'my_value');
```

Check if selected

```php
$option = $this->getSession()->getPage()
    ->find('css', '[name="my_name"][value="my_value"]');
assertEquals('checked', $option->getAttribute('checked'));
```
