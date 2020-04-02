Fonction JS:

```
function switchTheme(event) {
    if (event.target.checked) {
        document.documentElement.setAttribute('data-theme', 'dark');
        localStorage.setItem('dark-mode', 'dark');
    }
    else {
        document.documentElement.setAttribute('data-theme', 'light');
        localStorage.setItem('dark-mode', 'light');
    }    
}

const darkMode = localStorage.getItem('dark-mode');
document.documentElement.setAttribute('data-theme', darkMode);

const toggler = document.querySelector('#toggler')
```
