Behat Reference
===============


## Mink

### Radio button

Select a radio button

```php
$this->selectOption('my_name', 'my_value');
```

Assert is selected

```php
$option = $this->getSession()->getPage()->find('css', '[name="my_name"][value="my_value"]');
assertEquals('checked', $option->getAttribute('checked'));
```

### Check box

Check a checkbox

```php
$this->checkOption('my_name');
```

Uncheck a checkbox


```php
$this->uncheckOption('my_name');
```
