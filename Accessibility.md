# Accessibility

_*All APT web projects should be as accessible as possible to the largest population*_

## Skip links

* Skip links allow users to skip straight to the #main-content, providing content that can be accessed more quickly
  * put this link at the top of the RootLayout.jsx component

``` html
  <a href='#main-content' className='skip-link'>Skip to main content</a>
```

  * include this styling in _general.scss
  
  ```scss
  .skip-link {
    position: absolute;
    top: -40px;
    left: 0;
    background: #000;
    color: white;
    padding: 8px;
    z-index: 100;

    &:focus {
      top: 0;
    }
  } 
  ```

## Linked images with alternative descriptive text

  ```jsx
  <div className='hero-container' role='article' aria-label={`Program information for ${program.title}`}>
  ```

## aria-labels on object properties and video windows

  ```jsx
  aria-label='{variable}'
  ```

## Tabindex on actionable items

  ```jsx
  tabIndex='0'
  ``` 

## Contrast increased on view buttons and font made bolder

